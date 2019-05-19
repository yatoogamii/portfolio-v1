<template>
  <article class="about__img-container">
    <img class="about__img" src="../../../public/code.jpg" alt="setup de code"/>
  </article>
</template>

<script>
export default{
  name: 'Img'
}
</script>

<style lang="scss" scoped>
.about__img-container {
  width: 50%;
  height: 100%;

  .about__img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    object-position: center;
  }
}
</style>

