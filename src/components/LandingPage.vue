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
                        <div class="mobile-menu">
                            
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
        <footer>
            <p>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Orci a scelerisque purus semper eget. Sed vulputate odio ut enim blandit. Cras semper auctor neque vitae tempus quam pellentesque nec. Amet volutpat consequat mauris nunc congue nisi.
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
        background-color: #fafafa;
    }
    .counter {
        max-width: 500px;
        overflow: auto;
        min-height: 200px;
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

    @keyframes blinker {
    50% {
        opacity: 0;
    }
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
    }
</style>