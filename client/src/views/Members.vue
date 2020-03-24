<template>
<div class="container">
	<div class="row">
		<div class="container">
            <div class="col-12 text-center pt-3">
                <h1>NBA Community Members</h1>
            </div>
            <hr class="bg-dark mt-5 mb-5 w-25">
            <form class="form-inline my-2 my-lg-0">
                <input class="form-control m-auto" type="text" placeholder="Search" aria-label="Search" style="width: 300px; text-align: center;">
            </form>
            <div class="row">
                <div class="col-md-4 mb-5 mt-5">
                    <div class="card mb">
                    <img class="card-img-top" src="../assets/mem1.png" alt="Card image cap">
                    <div class="card-body mb">
                        <h5 class="card-title">Giannis Antetokounmpo</h5>
                        <p class="card-text">9200 N Upper River Rd<br />Milwaukee, WI 53217<br><br>giannis_an34@gmail.com</p>
                        <button type="button" class="btn btn-primary mb m-3">View</button>
                        <button type="button" class="btn btn-primary mb m-3">Add Friend</button>
                    </div>
                    </div>
                </div>
                <div class="col-md-4 mb-5 mt-5">
                    <div class="card mb">
                    <img class="card-img-top" src="../assets/mem2.png" alt="Card image cap">
                    <div class="card-body mb">
                        <h5 class="card-title">LeBron James</h5>
                        <p class="card-text">555 N Nash St.<br />El Segundo, CA 90245<br><br>kingjames@gmail.com</p>
                        <button type="button" class="btn btn-primary mb m-3">View</button>
                        <button type="button" class="btn btn-primary mb m-3">Add Friend</button>
                    </div>
                    </div>
                </div>
                <div class="col-md-4 mb-5 mt-5">
                    <div class="card mb">
                    <img class="card-img-top" src="../assets/mem3.png" alt="Card image cap">
                    <div class="card-body mb">
                        <h5 class="card-title">James Harden</h5>
                        <p class="card-text">11706 Empress Oaks Ct<br />Houston, TX 77082<br><br>jharden13@gmail.com</p>
                        <button type="button" class="btn btn-primary mb m-3">View</button>
                        <button type="button" class="btn btn-primary mb m-3">Add Friend</button>
                    </div>
                    </div>
                </div>
                <div class="col-md-4 mb-5">
                    <div class="card mb">
                    <img class="card-img-top" src="../assets/mem4.png" alt="Card image cap">
                    <div class="card-body mb">
                        <h5 class="card-title">Anthony Davis</h5>
                        <p class="card-text">9 Forrest Ct<br />Metairie, LA 70001<br><br>antdavis23@gmail.com</p>
                        <button type="button" class="btn btn-primary mb m-3">View</button>
                        <button type="button" class="btn btn-primary mb m-3">Add Friend</button>
                    </div>
                    </div>
                </div>
                <div class="col-md-4 mb-5">
                    <div class="card mb">
                    <img class="card-img-top" src="../assets/mem5.png" alt="Card image cap">
                    <div class="card-body mb">
                        <h5 class="card-title">Luka Dončić</h5>
                        <p class="card-text">2500 Victory<br />AveDallas, TX 75201<br><br>luka7doncic@gmail.com</p>
                        <button type="button" class="btn btn-primary mb m-3">View</button>
                        <button type="button" class="btn btn-primary mb m-3">Add Friend</button>
                    </div>
                    </div>
                </div>
                <div class="col-md-4 mb-5">
                    <div class="card mb">
                    <img class="card-img-top" src="../assets/mem6.png" alt="Card image cap">
                    <div class="card-body mb">
                        <h5 class="card-title">Kawhi Leonard</h5>
                        <p class="card-text">6130 Lago Lindo<br />Rancho Santa Fe, CA 92067<br><br>kawhileonard@gmail.com</p>
                        <button type="button" class="btn btn-primary mb m-3">View</button>
                        <button type="button" class="btn btn-primary mb m-3">Add Friend</button>
                    </div>
                    </div>
                </div>
            </div>
        </div>
	</div>
</div>
</template>

<style>
.mb.card-body{
    text-align: center;
}
.mb.btn{
    border-radius: 0;
    box-shadow: 0.5px 1px 2px hsla(0, 0%, 20%, 1);
}
.mb.btn:hover{
    transform: translateY(-2px);
    box-shadow: 2px 2px 5px hsla(0, 0%, 20%, 1);
}
.mb.card{
    border-radius: 0px / 0px;
    overflow: hidden;
    box-shadow: 0.5px 1px 2px hsla(0, 0%, 20%, 1);
}
.card-title {
    font-weight: 700;
}
</style>