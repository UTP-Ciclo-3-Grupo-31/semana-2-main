<template>
     <div id="services" class="section-1">
        <div class="services-card">
            <div class="services-image">
                <img src="../assets/web_dev_icon2.png" alt="" srcset="">
            </div>
            <div class="services-card-content">
                <br>
                <h5 class="services-card-title">Desarrollo Web</h5>
                <br>
                <p class="services-card-description">Servicio de desarrollo web personalizado.</p>
                <br>
                <br>
                <a class="services-card-link" href="web_dev.html">Más info acá</a>
            </div>
        </div>

        <div class="services-card">
            <div class="services-image">
                <img src="../assets/cloud_icon3.png" alt="" srcset="">
            </div>
            <div class="services-card-content">
                <br>
                <h5 class="services-card-title">Almacenamiento en la nube</h5>
                <br>
                <p class="services-card-description">Ofrecemos servicio de almacenamiento en la nube para tu web y su base de datos.</p>
                <br>
                <br>
                <a  class="services-card-link" href="cloud.html">Más info acá</a>
            </div>
        </div>

        <div class="services-card">
            <div class="services-image">
                <img src="../assets/web_advertising_icon.png" alt="" srcset="">
            </div>
            <div class="services-card-content">
                <br>
                <h5 class="services-card-title">Publicidad web</h5>
                <br>
                <p class="services-card-description">Ofrecemos servicio de publicidad en las noticias de tecnología de nuestra web.</p>
                <br>
                <br>
                <a  class="services-card-link" href="publicidad.html">Más info acá</a>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: "Services",
        props: ['service']
    }
</script>

<style scoped>

.section-1 {
    width: 100%;
    
    display: flex;
    justify-content: space-around;
    background-color: rgb(21, 37, 107);
    padding: 2%;
    align-items: center;
    /* margin: 2%; */
    /*
    margin-top: 10vh;
    */
}

.services-card {
    width: 25%;
    /* height: 100%; */
    background-color: #ffffff;
    justify-content: center;
    border-radius: 25px;
    box-shadow: 0px 20px 20px 10px rgba(0, 0, 0, 0.2);
    padding: 1%;

    transition: 0.5s ease;
    cursor: pointer;
}

.services-card:hover{
    transform: scale(1.06);
    box-shadow: 0px 20px 20px 10px rgba(0, 0, 0, 0.4);

}

.services-card img{
    width: 75%;
    padding:30px;
    /*height: 50%;*/
    justify-self: center;
    display: block;
    margin: auto;
    
}

.services-card .services-image{
    width: 100%;
    border-radius: 23px 23px 130px 130px;
    background-color: #25a3f7
}


.services-card .services-card-title {
    width: 80%;
    height: auto;
    margin: auto;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    text-align: center;
    color: #0c0629;
}

.services-card .services-card-description {
    width: 80%;
    height: auto;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    text-align: center;
    margin: auto;
    color: #0d2e53;

}

.services-card .services-card-link {
    width: 80%;
    height: auto;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    text-align: center;
    font-size: 2rem;
    margin: auto;
    color: #0d2e53;

}
</style>