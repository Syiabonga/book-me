<template>
    <div class="conatiner-fluid">
        <div class="main-banner">
            <div class="menu">
                <nav class="navbar navbar-expand-lg">
                    <div class="container-fluid">
                        <strong>
                            <a class="navbar-brand" href="#">BarberShop</a>
                        </strong>
                        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarText" aria-controls="navbarText" aria-expanded="false" aria-label="Toggle navigation">
                        <span class="navbar-toggler-icon"></span>
                        </button>
                        <div class="collapse navbar-collapse" id="navbarText">
                        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                            <li class="nav-item">
                            <a class="nav-link active" aria-current="page" href="#">Barbers</a>
                            </li>
                            <li class="nav-item">
                            <a class="nav-link" href="#">All Appointments</a>
                            </li>
                        </ul>
                        <span class="navbar-text">
                            Login
                        </span>
                        </div>
                    </div>
                </nav>
            </div>
            <div class="text-center">
                <h1>More than just a haircut</h1>
                <h1>A life style</h1>
                <button type="button" class="btn btn-primary">Book an appoitment</button>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name: 'compLandingPage'
}
</script>
<style >
    .main-banner{
        background-color: #090F1A;
        color:white;
        background-image: url("../assets/barber.svg");
        height: 500px;
        background-size: contain;
        background-repeat: no-repeat;
        background-position: center;
    }
    nav a{
        color: white !important;
    }
    nav ul{
        margin-left: 100px;
    }
    nav ul li{
        margin: 5px;
    }
    nav ul li a:hover{
        color: #4D78CA !important;
    }
    .text-center{
        text-align: left !important;
        padding: 10%;
        font-weight: bolder;
    }
    .text-center button{
        background-color: #6096FD !important;
        border: #6096FD;
        border-radius: 0;
        width: 200px;
        height: 50px;
    }
    .text-center button:hover{
        background-color: #4D78CA !important;
        transition: 0.5s;
    }
</style>