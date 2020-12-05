<template>
  <div id="app">
    <services></services>
    <noticias></noticias>
    <team-card></team-card>
  </div>
</template>

<script>

import Services from './components/Services.vue'
import TeamCard from './components/TeamCard.vue'
import Noticias from './components/Noticias.vue'

export default {
  name: 'App',
  components:{
    Services,
    TeamCard,  
    Noticias,
  }
}
</script>

<style>

</style>

