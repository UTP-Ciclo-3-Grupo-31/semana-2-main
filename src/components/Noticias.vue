<template>
    <div class="container-fluid" id="noticias">
        <div class="row justify-content-center mt-5 ">
            <div class="col-5 bg-light border rounded ml-4 mb-4" v-for="(noticia,key) in news" :key="key" >
                <h5 >
                {{ noticia[0]}}
                </h5>
                <div class="row justify-content-center">
                    <img class="img-fluid img-noticia" :src="noticia[2]">
                </div>
                <p>
                    {{ noticia[1]}}
                </p>
                <div class="row">
                    <a class="col" target="_blank" v-bind:href="noticia[3]">leer mas...</a>
                    <h5 class="col" >publicado el {{noticia[4]}}</h5>
                </div>
            </div>
        </div>
    </div>
</template>

<script>

const cantidadArticulos = 4;
var listadoArticulos = [];

const obtenerArticulos = async () => {
    const resultText = await fetch('http://newsapi.org/v2/top-headlines?country=co&apiKey=5f3c419ec6044044ac2462c9ad164194' ,{
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
    width: 60%;
}
</style>
