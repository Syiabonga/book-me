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
                        <ul class="nav navbar-nav navbar-right">
                            <li><a href="#"><span class="glyphicon glyphicon-user"></span> Sign Up</a></li>
                            <li><a href="#"><span class="glyphicon glyphicon-log-in"></span> Login</a></li>
                        </ul>
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
        <div class="section-counter">
            <div class="counter">
            <center>
                <h1 class="blink-me">38</h1>
                <h2>Costumers at the location</h2>
            </center>
        </div>
        </div>
        <div class="usage-section">
            <div class="row tex-center">
                <div class="col-md-4">
                    <img src="../assets/time.png" alt="">
                    <p>
                        Avoid waiting to get a haircut
                    </p>
                </div>
                <div class="col-md-4">
                    <img src="../assets/barber.png" alt="">
                    <p>
                        Pick your favorite barber in advance
                    </p>
                </div>
                <div class="col-md-4">
                    <img src="../assets/feedback.png" alt="">
                    <p>
                        Let the others know what you think about your barber
                    </p>
                </div>
            </div>
        </div>
        <footer>
            <p>
                © 2021 BookMe. All rights reserved.
            </p>
        </footer>
    </div>
</template>
<script>
export default {
    name: 'compLandingPage'
}
</script>
<style lang="scss">
    $bg-banner: #090F1A;
    $costumer-counter-color: #6096FD;
    $section-background: #fafafa;
    .main-banner{
        background-color: $bg-banner;
        color:white;
        background-image: url("../assets/barber.svg");
        height: 500px;
        background-size: contain;
        background-repeat: no-repeat;
        background-position: center;
    }
    nav{
        padding: 50px;
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
    .section-counter{
        background-color: $section-background;
        min-height: 200px;
        margin-top: 20px;
    }
    .section-counter h1{
        font-size: 50px;
    }
    .counter {
        max-width: 500px;
        overflow: auto;
        margin: auto;
        padding: 30px;
        border-radius: 5px;
    }
    .counter h1{
        color: $costumer-counter-color;
    }
    .blink-me {
        animation: blinker 1s linear infinite;
    }
    .usage-section{
        background-color: $section-background;
        padding: 50px;
    }
    .usage-section img{
        display: block;
  margin-left: auto;
  margin-right: auto;
    }
    .usage-section p{
        font-size: 20px;
        text-align: center;
        margin-top: 10px;
    }
    @keyframes blinker {
    50% {
        opacity: 0;
    }
    }
    footer{
        background-image: linear-gradient(76deg, #020f1f, #0f0d2e);
        color: white;
        height: 100px;
    }
    footer p{
        text-align: center;
        padding: 20px;
    }







    @media only screen and (max-width: 600px) {
        nav{
            padding: 10px;
        }
        h1{
            font-size: 30px !important;
        }
        .main-banner{
            padding: 20px;
        }
        .text-center{
            margin-top: 40px;
            font-weight: 900;
        }
        .section-counter{
            padding: 20px;
        }
        .section-counter h1{
            font-size: 50px !important;
        }
        .usage-section{
            padding-top: 0;
        }
        .usage-section .col-md-4{
            margin-top: 30px;
        }
    }
</style>