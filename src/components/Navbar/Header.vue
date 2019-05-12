<template>
  <header class="Navbar-container__title">
    <h1 class="Navbar-container__title-h1">Bracaval Elias</h1>
    <h2 class="Navbar-container__title-h2">Developer Full Stack Junior</h2>
  </header>
</template>

<script>
export default{
  name: 'Header'
}
</script>

<style lang="scss" scoped>

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
</style>

