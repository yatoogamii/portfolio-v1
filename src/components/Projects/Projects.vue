<template>
  <section id="project" class="project">
    <Project>
    <template v-slot:img>
      <img src="../../assets/img/score-keeper.png" alt="preview site"/>
    </template>
    <template v-slot:text>
      <h1>Score Keeper</h1>
      <p class="div-project__desc">Jeux réalisé en Js Vanilla où deux joueurs s'affrontent pour atteindre un score maximum</p>
      <p class="div-project__tag text--red">#HTML #CSS #JS #Nostalgic-css</p>
    </template>
    </Project>
    <Project textalign="text-align: right">
    <template v-slot:img>
      <img src="../../assets/img/quotation.png" alt="preview site"/>
    </template>
    <template v-slot:text>
      <h1>Quotation</h1>
      <p class="div-project__desc">Application réalisé sans Js native qui génère des citations aléatoires depuis une API</p>
      <p class="div-project__tag text--red">#HTML #CSS #ReactJS #Axios #MaterialUI</p>
    </template>
    </Project>
  </section>
</template>

<script>
import Project from './Project.vue';

export default{
  name: 'Projects',
  components: {
    Project
  }
}
</script>

<style lang="scss" scoped>

.project {
  width: 100vw;
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
}

</style>
