<template>
  <section id="about" class="about">
    <Img></Img>
    <TextAbout></TextAbout>
  </section>
</template>

<script>
import Img from './Img.vue';
import TextAbout from './TextAbout.vue';

  export default{
    name: 'About',
    components: {
      Img,
      TextAbout
    }
  }
</script>

<style lang="scss" scoped>
.about {
  width: 100vw;
  height: 100vh;
  display: flex;
  flex-wrap: wrap;
  align-items: center;
}
</style>

