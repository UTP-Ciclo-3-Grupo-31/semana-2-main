<template>
  <div id="app">
    <header-page></header-page>
    <services></services>
    <noticias></noticias>
    <team-card></team-card>
    <footer-page></footer-page>
  </div>
</template>

<script>

import HeaderPage from './components/HeaderPage.vue'
import Services from './components/Services.vue'
import TeamCard from './components/TeamCard.vue'
import Noticias from './components/Noticias.vue'
import FooterPage from './components/FooterPage.vue'

export default {
  name: 'App',
  components:{
    HeaderPage,
    Services,
    TeamCard,  
    Noticias,
    FooterPage,
  }
}
</script>

<style>

</style>

