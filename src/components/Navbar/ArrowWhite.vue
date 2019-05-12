<template>
  <a href="#">
    <div :style="top" class="Navbar-container__arrow-white"></div>
  </a>
</template>

<script>
  export default{
    name: 'ArrowWhite',
    props: ['top'],
  }
</script>

<style lang="scss" scoped>

  .Navbar-container__arrow-white {
    position: absolute;
    background-color: #d2d2d4;
    left: 50%;
    transform: translate(-50%);
    width: 13vw;
    height: 13vw;
    clip-path: polygon(50% 100%, 0 50%, 0 49%, 50% 99%, 100% 49%, 100% 50%);
    z-index: 1;
  }

</style>

