<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <Person name="Zhymir Thompson" :about="about"></Person>
    <Links :links="links"></Links>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import Person from './components/Person.vue';
import Links from './components/Links.vue';
import about from './assets/about.js';
import links from './assets/links.js';

export default {
  name: 'App',
  components: {
    // HelloWorld,
    Person,
    Links
  },
  data() {
    return {
      about: about,
      links: links
    }
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
