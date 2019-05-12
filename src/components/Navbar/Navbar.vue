<template>
  <header class="Navbar-container">
    <NavbarLeft></NavbarLeft>
    <Header></Header>
    <NavbarRight></NavbarRight>
    <ArrowWhite top="top: 30vh"></ArrowWhite>
    <ArrowWhite top="top: 48vh"></ArrowWhite>
    <ArrowWhite top="top: 66vh"></ArrowWhite>
  </header>
</template>

<script>
import NavbarRight from './NavbarRight.vue';
import NavbarLeft from './NavbarLeft.vue';
import Header from './Header.vue';
import ArrowWhite from './ArrowWhite.vue';

export default{
  name: 'Navbar',
  components: {
    NavbarLeft,
    NavbarRight,
    Header,
    ArrowWhite
  }
}
</script>

<style lang="scss" scoped>
.Navbar-container {
  width: 100vw;
  height: 100vh;
}
</style>

