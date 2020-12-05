<template>
  <div id="app">
    <header-page></header-page>
    <services></services>
    <noticias></noticias>
    <div class="container">
      <div class="row justify-content-center mb-5">
        <div class="col mt-2" v-for="(item, key) of team" :key="key">
          <team-card :member="item"></team-card>
        </div>
      </div>
    </div>
    <footer-page></footer-page>
  </div>
</template>

<script>
import HeaderPage from "./components/HeaderPage.vue";
import Services from "./components/Services.vue";
import TeamCard from "./components/TeamCard.vue";
import Noticias from "./components/Noticias.vue";
import FooterPage from "./components/FooterPage.vue";

export default {
  name: "App",
  components: {
    HeaderPage,
    Services,
    TeamCard,
    Noticias,
    FooterPage,
  },
  data() {
    return {
      team: [
        {
          codigo: 1,
          nombre: "Sergio Vargas",
          descripcion:
            "Programador,vive en Bogotá, le gusta Jugar con electrónica, volar drones y le apasionan las motos",
          rol: "Desarrollador backend",
          image: "https://placeimg.com/150/87/any",
        },
        {
          codigo: 2,
          nombre: "Diego Lipez",
          descripcion:
            "Ingeniero electricista de la Universidad Industrial de Santander, nacido en Bucaramanga actualmente vive en Bogotá, le gustan las caminatas por el campo y jugar minecraft con su hija.",
          rol: "Desarrollador backend",
          image: "https://placeimg.com/151/90/any",
        },
        {
          codigo: 5,
          nombre: "Engie Lorena Hernandez",
          descripcion:
            "Bogotana, tecnologa en gastronomia de la Universitaria Agustiniana, creativa, vive en busqueda constante de conocimiento, casada tiene una hija, apasionada por el arte, vive en la ciudad de Bogota y le gusta explorar rincones gastronomicos poco conocidos de esta ciudad.",
          rol: "Desarrollador frontend",
          image: "https://placeimg.com/148/89/any",
        },
        {
          codigo: 3,
          nombre: "Jose del Valle",
          descripcion:
            "Ingeniero de Control de la Universidad Nacional de Colombia, nacido en Itagüí vive actualmente en Medellín le gusta jugar vídeo juegos.",
          rol: "Desarrollador backend",
          image: "https://placeimg.com/152/91/any",
        },
        {
          codigo: 4,
          nombre: "Esteban Durán",
          descripcion:
            "Ingeniero Químico de la Universidad de Antioquia, vive en Medellín, le gusta hacer deporte, leer y el cine.",
          rol: "Desarrollador backend",
          image: "https://placeimg.com/149/92/any",
        },
      ],
    };
  },
};
</script>

<style>
</style>

