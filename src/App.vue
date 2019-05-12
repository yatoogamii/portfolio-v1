<template>
  <Arrow></Arrow>
</template>

<script>
import Arrow from './components/Arrow/Arrow.vue';

export default {
  name: 'App',
  components: {
    Arrow, 
  },
  data () {
    return {
    }
  }
}
</script>

<style lang="scss">
* {
  padding: 0;
  margin: 0;
  border: 0;
  box-sizing: border-box;
}

html {
  font-size: 62.5%;
}

body {
  background-color: #1d1d1d;
}


</style>
