<template>
 
  <rich />
<users></users>

<!--<name></name>--> 
  
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import home from './components/home.vue'
import loopsss from './components/loops.vue'
import rich from './components/compo.vue'
import name from './components/template.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    home,
    loopsss,
    rich,
    name

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
