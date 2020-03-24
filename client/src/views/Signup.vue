<template>
    <div class="sign-up" @submit.prevent = 'register'>
        <div class="container">
            <div class="row h-100 justify-content-center">
                <div class="text-box col-md-5" id="sign-up-box">
                    <form>
                        <h2>Create an Account</h2>
                        <div class="form-group text-center">
                            <label for="first_name">First Name</label>
                            <input type="text" class="form-control" name="fname" id="fname" placeholder="First Name" v-model="fname"/>
                        </div>
                        <div class="form-group text-center ">
                            <label for="middle_name">Middle Initial</label>
                            <input type="text" class="form-control" name="mname" id="mname" placeholder="Middle Initial" v-model="mname"/>
                        </div>
                        <div class="form-group text-center">
                            <label for="last_name">Last Name</label>
                            <input type="text" class="form-control" name="lname" id="lname" placeholder="Last Name" v-model="lname"/>
                        </div>
                        <div class="form-group text-center">
                            <label for="last_name">Mobile No.</label>
                            <input type="tel" pattern="[0-9]{11}" class="form-control" name="mobilenum" id="mobilenum" placeholder="Mobile No." v-model="mobilenum"/>
                        </div>
                        <div class="form-group text-center ">
                            <label for="birthdate">Birthdate</label>
                            <input type="date" class="form-control" name="bdate" id="bdate" placeholder="Birthdate" v-model="bdate"/>
                        </div>
                        <div class="form-group text-center">
                            <label for="address">Address</label>
                            <textarea type="text" class="form-control" name="address" id="address" placeholder="Address" v-model="address"/>
                        </div>
                        <div class="form-group text-center">
                            <label for="email_address">Email Address</label>
                            <input type="email" class="form-control" name="email" id="email" placeholder="Email Address" v-model="email"/>
                        </div>
                        <div class="form-group text-center ">
                            <label for="password">Password</label>
                            <input type="password" class="form-control" name="password" id="password" placeholder="Password" v-model="password"/>
                        </div>
                        <div class="form-group text-center">
                            <label for="confirm_password">Confirm Password</label>
                            <input type="password" class="form-control" name="cpass" id="cpass" placeholder="Confirm Password" v-model="cpass"/>
                        </div>
                        <div class="form-group">
                            <button class="btn btn-lg btn-success m-3" type="submit"> Register </button>
                            <button class="btn btn-lg btn-danger m-3" type="button"> Cancel </button>
                        </div>
                    </form>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    import axios from 'axios'
    import router from '../router'
    export default {
        data () {
            return {
                fname:'',
                mname:'',
                lname:'',
                mobilenum:'',
                address:'',
                bdate:'',
                sex:'',
                email:'',
                username:'',
                password:'',
                cpass:''
            }
        },
        methods: {
            register () {
                axios.post('app/signup', {
                    first_name:this.fname,
                    middle_initial:this.mname,
                    last_name:this.lname,
                    mobile_no:this.mobilenum,
                    address:this.address,
                    birthdate:this.bdate,
                    sex:this.sex,
                    email_address:this.email,
                    username:this.username,
                    password:this.password,
                }).then(res => {
                    if (!res.data){
                        alert('You have successfully registered...')
                        router.push({name: 'Home'})
                    }
                }).catch(err => {
                    console.log(err)
                })
            }
        }
    }
</script>