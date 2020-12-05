<template>
    <div class="container" id="noticias">
        <div class="row">
            <div class="col-md-6" v-for="noticia in news" :key="noticia" >
                <h5 >
                {{ noticia[0]}}
                </h5>
                <img class=" img-noticia" :src="noticia[2]">
                <p>
                    {{ noticia[1]}}
                </p>
                <div class="row">
                    <a class="col-5" target="_blank" v-bind:href="noticia[3]">leer mas...</a>
                    <h5 class="col-5" >publicado el {{noticia[4]}}</h5>
                </div>
            </div>
        </div>
    </div>
</template>

<script>

const cantidadArticulos = 4;
var listadoArticulos = [];

const obtenerArticulos = async () => {
    const resultText = await fetch('http://newsapi.org/v2/top-headlines?country=co&category=technology&apiKey=5f3c419ec6044044ac2462c9ad164194' ,{
    method:'GET',
    });
    let articulosJSON = await resultText.json();
    if(resultText.ok){
        for (let index = 0; index < cantidadArticulos; index++) {
            listadoArticulos.push([
                articulosJSON.articles[index].title,
                articulosJSON.articles[index].description,
                articulosJSON.articles[index].urlToImage,
                articulosJSON.articles[index].url,
                articulosJSON.articles[index].publishedAt,
                                ])
        }
    }
}
obtenerArticulos();

    export default {
        name: "Noticias",
        props: ['noticia'],
        data(){
            return{
                news: listadoArticulos,
                }
            }
    }
</script>

<style scoped>

.img-noticia{
    width: 70%;
}
</style>
