<template>
    <nav class="Navbar-container__nav Navbar-container__nav-right elevation-12">
      <a class="Navbar-container__nav__link Navbar-container__nav-right__link Navbar-container__link-project" href="#project">Project</a>
      <a class="Navbar-container__nav__link Navbar-container__nav-right__link Navbar-container__link-skills" href="#skills">Skills</a>
    </nav>
</template>

<script>
  export default{
    name: 'NavbarRight'
  }
</script>

<style lang="scss" scoped>

.Navbar-container__nav {
  display: flex;
  align-items: center;
  width: 35vw;
  height: 2.5vw;
  position: fixed;
  background-color: #bdbdbf;
  font-size: calc(1.5rem + 0.5vw);
  z-index: 1;
}

.Navbar-container__nav-right {
  padding: 0 1rem 0 5rem;
  right: 0;

  .Navbar-container__link-skills {
    position: fixed;
    right: 25%;
  }
  .Navbar-container__link-project {
    position: fixed;
    right: 16%;
  }
}

.Navbar-container__nav__link {
    position: relative;
    text-decoration: none;
    color: #1d1d1d;
}

</style>

