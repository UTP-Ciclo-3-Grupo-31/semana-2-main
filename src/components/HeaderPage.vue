<template>
    <header>
        <div class="flex-container">
            <div class="flex-item">
                <img src="../assets/codeLogo.png">
            </div>
            <h2>Equipo 31<br>Aprender es querer</h2>
            <nav class="flex-item" id="home">
                <ul>
                    <li class="btn btn-primary item"><a href="#home">Inicio</a></li>
                    <li class="btn btn-primary item"><a href="#services">Servicios</a></li>
                    <li class="btn btn-primary item"><a href="#news">Noticias</a></li>
                    <li class="btn btn-primary item"><a href="#team">Equipo</a></li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
    export default {
        name: "HeaderPage",
        props: ['header'],
        data(){
            return{
               
                }
            }
    }
</script>

<style scoped>
    header{
        background: url(../assets/banner.jpg);
    }
    header img{
        width: 100px;
    }
    header h2{
        color: white;
    }

    .container {
        width: 1200px;
        background-color: rgb(181, 223, 223);
        height: auto;
        -ms-flex-item-align: center;
        align-self: center;
        margin: 0px auto;
        padding: 0 auto;
    }

    .flex-container{
        display: flex;
        flex-flow: row;
        justify-content: space-around;
        align-items: center;
        height: 200px;
    }
    header a{
        color: white;
        }

</style>
