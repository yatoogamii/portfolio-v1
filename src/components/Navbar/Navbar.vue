<template>
  <section class="Navbar-container">
    <NavbarLeft toogleBool="toogleBool"></NavbarLeft>
    <Header toogleBool="toogleBool" :count="count" :link="link"></Header>
    <NavbarRight></NavbarRight>
    <ArrowWhite top="top: 30vh"></ArrowWhite>
    <ArrowWhite top="top: 48vh"></ArrowWhite>
    <ArrowWhite top="top: 66vh"></ArrowWhite>
  </section>
</template>

<script>
import NavbarRight from './NavbarRight.vue';
import NavbarLeft from './NavbarLeft.vue';
import Header from './Header.vue';
import ArrowWhite from './ArrowWhite.vue';

export default{
  name: 'Navbar',
  props: ['link', 'count'],
  components: {
    NavbarLeft,
    NavbarRight,
    Header,
    ArrowWhite
  },
  data() {
    return {
      toogleBool: true
    };
  }
  
}
</script>

<style lang="scss" scoped>
.Navbar-container {
  width: 100vw;
  height: 100vh;
}
</style>

