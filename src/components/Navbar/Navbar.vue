<template>
  <div class="Navbar-container">
    <nav class="Navbar-container__nav Navbar-container__nav-left">
      <a class="Navbar-container__nav__link Navbar-container__nav-left__link Navbar-container__link-contact" href="#" target="_blank">Contact</a>
      <a class="Navbar-container__nav__link Navbar-container__nav-left__link Navbar-container__link-about" href="#" target="_blank">About</a>
    </nav>
    <header class="Navbar-container__title">
      <h1 class="Navbar-container__title-h1">Bracaval Elias</h1>
      <h2 class="Navbar-container__title-h2">Developer Full Stack Junior</h2>
    </header>
    <nav class="Navbar-container__nav Navbar-container__nav-right">
      <a class="Navbar-container__nav__link Navbar-container__nav-right__link Navbar-container__link-project" href="#" target="_blank">Project</a>
      <a class="Navbar-container__nav__link Navbar-container__nav-right__link Navbar-container__link-skills" href="#" target="_blank">Skills</a>
    </nav>
  </div>
</template>

<script>
  export default{
    name: 'Navbar'
  }
</script>

<style lang="scss" scoped>
.Navbar-container {
  display: flex;
  justify-content: center;
  margin: auto;
}

.Navbar-container__title {
  display: flex;
  flex-direction: column;
  position: fixed;
  width: 35vw;
  height: 20vw;
  text-align: center;
  background-color: #d2d2d4;
  color: #1d1d1d;
  clip-path: polygon(50% 100%, 0 0, 100% 0);
  z-index: 1;

  .Navbar-container__title-h1 {
    position: relative;
    font-size: 2vw;
    top: 4vw;
  }
  .Navbar-container__title-h2 {
    position: relative;
    font-size: 1.2vw;
    margin-top: 1rem;
    top: 4vw;
  }

}

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

