<template>
  <article class="container-coordonate">
    <div class="coordonate">
      <p>Mail : <a href="mailto:bracaval.elias.pro@gmail.com">bracaval.elias.pro@gmail.com</a></p>
      <p>Telephone: <a href="tel:+33618895016">06.18.89.50.16</a></p>
      <p>LinkekIn : <a href="https://www.linkedin.com/in/elias-bracaval-517678174/" target="_blank">Elias Bracaval</a></p>
      <p>Twitter : <a href="https://twitter.com/BracavalE" target="_blank">@bracavalE</a></p>
    </div>
  </article>
</template>

<script>
  export default{
    name: 'Coordonate'
  }
</script>

<style lang="scss" scoped>
.container-coordonate {
  grid-row: 2 / 3;
  grid-column: 4 / 5;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;

  .coordonate {
    width: 100%;
    height: 50%;
    border: 0.1rem solid #d1d1d1;
    font-size: 1.5rem;
    padding: 1rem;
    color: #d1d1d1;
  }
}
</style>

