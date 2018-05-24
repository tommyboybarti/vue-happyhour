<template>
  <div id="app">
    <img src="./assets/happy-hour-gray.png">
    <!-- using imported component as html tag -->
    <component v-bind:is="component" msg="This app makes you drink for cheap"/>
    <button v-on:click="component = 'welcome'">Show welcome</button>
    <button v-on:click="component = 'bar'">Show bar</button>
  </div>
</template>

<script>
// importing component locally
import HelloWorld from './components/HelloWorld.vue'
import One18 from './components/One18.vue'

export default {
  name: 'app',
  // reference to the imported comp
  components: {
    'welcome': HelloWorld,
    'bar': One18
  },
  data() {
    return {
      component: 'welcome'
    } 
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
#app img {
  width: 80%;
  max-width: 500px;
}
</style>
