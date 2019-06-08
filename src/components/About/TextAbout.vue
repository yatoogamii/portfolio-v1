<template>
  <article class="about__text-container">
    <h1 class="about__text-title">Apprenant <span class="about__text--red">professionnel</span></h1>
    <p class="about__text-desc">Je me présente, Elias Bracaval, 19 ans. Je suis sur un pc depuis l'âge de <span class="about__text--red">6 ans</span>, j'ai d'abord découvert le code en <span class="about__text--red">autodidacte</span> avant de me lancer dans une formation de <span class="about__text--red">développer Web</span>. Je suis actuellement en perpétuel recherche de <span class="about__text--red">nouveauté</span> dans le domaine </p>
    <p class="about__text-quote">The <span class="about__text--red">harder</span> i work, the <span class="about__text--red">luckier</span> i get</p>
  </article>
</template>

<script>
export default{
  name: 'TextAbout', 
}
</script>

<style lang="scss">

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
    font-size: 2rem;
    width: 80%;
    text-align: right;
  }

  .about__text-desc {
    font-size: 1.5rem;
    width: 80%;
  }

  .about__text-quote {
    font-size: 1rem;
    width: 80%;
    text-align: left;
  }

  .about__text--red {
    color: red;
  }
}

</style>

