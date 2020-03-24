<template>
    <div class="login">
        <div class="container">
            <div class="row h-100 justify-content-center align-items-center">
                <div class="text-box col-md-5" id="login-box">
                    <form>
                        <h2>Log In</h2>
                        <div class="form-group text-center">
                            <label for="email_address">Email Address</label>
                            <input type="email" class="form-control" name="email" id="email" placeholder="Email Address" v-model="email"/>
                        </div>
                        <div class="form-group text-center ">
                            <label for="password">Password</label>
                            <input type="password" class="form-control" name="password" id="password" placeholder="Password" v-model="password"/><br>
                            <input type="checkbox" id="remember" name="remember">
                            <label>Remember me</label><br>
                            <label>Not a member?</label>&nbsp;
                            <a href="/signup">Create an account.</a><br><br>
                            <button class="btn btn-lg btn-success m-3" type="submit"> Login </button>
                            <button class="btn btn-lg btn-danger m-3" type="button"> Cancel </button>
                        </div>
                    </form>
                </div>
            </div>
        </div>
    </div>
</template>


<style>
.login{
    height: 882px;
    background-image: linear-gradient(rgba(0,0,0,0.1),rgba(0,0,0,0.3)),url('../assets/bg2.jpg');
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
}
.sign-up{
    background-image: linear-gradient(rgba(0,0,0,0.1),rgba(0,0,0,0.3)),url('../assets/bg.jpg');
    background-position: center;
    background-size: cover;
}

.text-box{
    color: snow;
    background: rgba(0,0,0,0.6);
    margin: 70px 0 70px;
    padding: 50px;
}

#login-box{
    margin: 15%;
}

form h2{
    margin-bottom: 50px;
}

input[type="radio"], input[type="checkbox"]{
  margin: 0 10px 0 10px;
}
</style>