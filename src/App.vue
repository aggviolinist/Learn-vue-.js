<template>
 
 <rich />
 <users></users>

 
  
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import home from './components/home.vue'
import loopsss from './components/loops.vue'
import rich from './components/compo.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    home,
    loopsss,
    rich

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
