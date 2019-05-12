<template>
  <div class="arrow-container">
    <nav class="arrow-container__nav arrow-container__nav-left">
      <a class="arrow-container__nav__link arrow-container__nav-left__link" href="#" target="_blank">Skills</a>
    </nav>
    <header class="arrow-container__title">
      <h1>Bracaval Elias</h1>
      <h2>Developer Full Stack Junior</h2>
    </header>
    <nav class="arrow-container__nav arrow-container__nav-right">
      <a class="arrow-container__nav__link arrow-container__nav-right__link" href="#" target="_blank">About</a>
    </nav>
  </div>
</template>

<script>
  export default{
    name: 'Arrow'
  }
</script>

<style lang="scss" scoped>
.arrow-container {
  display: flex;
  justify-content: center;
  margin: auto;
}

.arrow-container__title {
  position: fixed;
  width: 35vw;
  height: 20vw;
  text-align: center;
  background-color: #e6e6e9;
  color: #1d1d1d;
  clip-path: polygon(50% 100%, 0 0, 100% 0);
  z-index: 1;
}

.arrow-container__nav {
  display: flex;
  align-items: center;
  width: 35vw;
  height: 3rem;
  position: fixed;
  background-color: #d2d2d4;
  font-size: 2rem;
}

.arrow-container__nav-left {
  padding: 0 5rem 0 1rem;
  left: 0;

  .arrow-container__nav-left__link {
    margin-right: auto;
  }
}
.arrow-container__nav-right {
  padding: 0 1rem 0 5rem;
  right: 0;

  .arrow-container__nav-right__link {
    margin-left: auto;
  }
}

.arrow-container__nav__link {
    position: relative;
    text-decoration: none;
    color: #1d1d1d;
}

</style>

