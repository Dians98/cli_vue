<template>
  <div id="app">
    <img src="./assets/logo.png" alt="">
    <mon-premier-composant></mon-premier-composant>
  </div>
</template>

<script>
import monPremierComposant from './components/mon-premier-composant.vue';

export default {
  name: 'App',
  /*  
    propriété qui permet d'enregistrer les composants locallement
  */
  components: {
    /**
     * 'nom d'utilisation dans ce fichier' : reference (par rapport à l'import)
     */
    'mon-premier-composant' : monPremierComposant
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
