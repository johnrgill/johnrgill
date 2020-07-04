<template>
  <div id="app">
    <navigation/>
    <router-view></router-view>
    
  </div>
</template>

<script>
import Navigation from './components/includes/navigation.vue' //import the component

export default {
  name: 'App',
  components: {
    Navigation  //instantiate it here
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
