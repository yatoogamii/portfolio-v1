<template>
  <article class="about__text-container">
    <h1 class="about__text-title">Apprenant <span class="about__text--red">professionnel</span></h1>
    <p class="about__text-desc">Je me présente, Elias Bracaval, 19 ans. Je suis sur un pc depuis l'âge de 6 ans, blablabla</p>
    <p class="about__text-quote">The <span class="about__text--red">harder</span> i work, the <span class="about__text--red">luckier</span> i get</p>
  </article>
</template>

<script>
export default{
  name: 'TextAbout', 
}
</script>

<style lang="scss" scoped>

.about__text-container {
  display: flex;
  align-items: center;
  justify-content: space-around;
  flex-direction: column;
  color: rgba(255, 255, 255, 1);
  font-size: 1.5rem;
  width: 50%;
  height: 80%;

  .about__text-title {
    width: 80%;
    text-align: right;
  }

  .about__text-desc {
    width: 80%;
  }

  .about__text-quote {
    width: 80%;
    text-align: left;
  }

  .about__text--red {
    color: red;
  }
}

</style>

