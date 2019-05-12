<template>
    <nav class="Navbar-container__nav Navbar-container__nav-right">
      <a class="Navbar-container__nav__link Navbar-container__nav-right__link Navbar-container__link-project" href="#" target="_blank">Project</a>
      <a class="Navbar-container__nav__link Navbar-container__nav-right__link Navbar-container__link-skills" href="#" target="_blank">Skills</a>
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
  height: 2.3vw;
  position: fixed;
  background-color: #bdbdbf;
  font-size: 1.5vw;
}

.Navbar-container__nav-right {
  padding: 0 1rem 0 5rem;
  right: 0;

  .Navbar-container__link-skills {
    position: fixed;
    right: 27.5%;
  }
  .Navbar-container__link-project {
    position: fixed;
    right: 20%;
  }
}

.Navbar-container__nav__link {
    position: relative;
    text-decoration: none;
    color: #1d1d1d;
}

</style>

