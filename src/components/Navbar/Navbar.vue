<template>
  <header class="Navbar-container elevation-24">
    <NavbarLeft></NavbarLeft>
    <Header></Header>
    <NavbarRight></NavbarRight>
    <ArrowWhite top="top: 15vw"></ArrowWhite>
    <ArrowWhite top="top: 24vw"></ArrowWhite>
    <ArrowWhite top="top: 33vw"></ArrowWhite>
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
  display: flex;
  justify-content: center;
  margin: auto;
}
</style>

