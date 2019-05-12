<template>
    <nav class="Navbar-container__nav Navbar-container__nav-left elevation-24">
      <a class="Navbar-container__nav__link Navbar-container__nav-left__link Navbar-container__link-contact" href="#" target="_blank">Contact</a>
      <a class="Navbar-container__nav__link Navbar-container__nav-left__link Navbar-container__link-about" href="#" target="_blank">About</a>
    </nav>
</template>

<script>
  export default{
    name: 'NavbarLeft'
  }
</script>

<style lang="scss" scoped>

.Navbar-container__nav {
  display: flex;
  align-items: center;
  width: 35vw;
  height: 2.3vw;
  position: fixed;
  background-color: #bdbdbf;
  font-size: 1.5vw;
}

.Navbar-container__nav-left {
  padding: 0 5rem 0 1rem;
  left: 0;

  .Navbar-container__link-about {
    position: fixed;
    left: 27%;
  }
  .Navbar-container__link-contact {
    position: fixed;
    left: 19%;
  }
}

.Navbar-container__nav__link {
    position: relative;
    text-decoration: none;
    color: #1d1d1d;
}

</style>

