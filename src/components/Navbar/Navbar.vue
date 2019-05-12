<template>
  <div class="Navbar-container">
    <NavbarLeft></NavbarLeft>
    <Header></Header>
    <NavbarRight></NavbarRight>
  </div>
</template>

<script>
import NavbarRight from './NavbarRight.vue';
import NavbarLeft from './NavbarLeft.vue';
import Header from './Header.vue';

export default{
  name: 'Navbar',
  components: {
    NavbarLeft,
    NavbarRight,
    Header
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

