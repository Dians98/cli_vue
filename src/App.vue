<template>
  <div id="app" class="container">
    <img src="./assets/logo.png" alt="">
    <welcome></welcome>
  </div>
</template>

<script>
import welcome from './components/welcome.vue';

export default {
  name: 'App',
  /*  
    propriété qui permet d'enregistrer les composants locallement
  */
  components: {
    /**
     * 'nom d'utilisation dans ce fichier' : reference (par rapport à l'import)
     */
    'welcome' : welcome
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
