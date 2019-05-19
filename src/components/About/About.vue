<template>
  <section class="about">
    <Img></Img>
    <Text></Text>
  </section>
</template>

<script>
import Img from './Img.vue';
import Text from './Text.vue';

  export default{
    name: 'About',
    components: {
      Img,
      Text
    }
  }
</script>

<style lang="scss" scoped>
.about {
  width: 100vw;
  height: 100vh;
}
</style>

