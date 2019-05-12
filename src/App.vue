<template>
  <Navbar></Navbar>
</template>

<script>
import Navbar from './components/Navbar/Navbar.vue';

export default {
  name: 'App',
  components: {
    Navbar, 
  }, 
  data() {
    return {
    }
  }
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
}

body {
  background-color: #1d1d1d;
  height: 200vh;
}


</style>
