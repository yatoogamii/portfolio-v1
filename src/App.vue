<template>
  <div>
    <Navbar :mousePos="mousePos"></Navbar>
    <About></About>
    <Skills></Skills>
  </div>
</template>

<script>
import Navbar from './components/Navbar/Navbar.vue';
import About from './components/About/About.vue';
import Skills from './components/Skills/Skills.vue';


export default {
  name: 'App',
  components: {
    Navbar, 
    About,
    Skills
  }, 
  data() {
    return {
      mousePos: 0,
    }
  },
}
</script>

<style lang="scss">
 @import url('https://fonts.googleapis.com/css?family=Raleway');

* {
  padding: 0;
  margin: 0;
  border: 0;
  box-sizing: border-box;
}

html {
  font-size: 62.5%;
  font-family: 'Raleway', sans-serif;
  scroll-behavior: smooth;
}

body {
  background-color: #1d1d1d;
}


</style>
