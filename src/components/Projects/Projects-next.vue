<template>
  <section id="project-next" class="project-next">
    <Project>
    <template v-slot:img>
      <img src="../../assets/img/photographe.png" alt="preview site"/>
    </template>
    <template v-slot:text>
      <h1>Photographe</h1>
      <p class="div-project__desc">Site vitrine pour une photographe spécialisé dans les naissances, l'enfance et les anniversaires</p>
      <p class="div-project__tag text--red">#HTML #CSS</p>
    </template>
    </Project>
    <Project textalign="text-align: right">
    <template v-slot:img>
      <img src="../../assets/img/monster-slayer.png" alt="preview site"/>
    </template>
    <template v-slot:text>
      <h1>Monster Slayer</h1>
      <p class="div-project__desc">Jeux réalisé sans Js native ou on peut faire affronter une personnage contre un boss, avec les possibilités d'utiliser des attaques spécials, de soigner et de recommencer</p>
      <p class="div-project__tag text--red">#HTML #CSS #VueJS #Vuetify</p>
    </template>
    </Project>
  </section>
</template>

<script>
import Project from './Project.vue';

export default{
  name: 'Projects-next',
  components: {
    Project
  }
}
</script>

<style scoped>
.project-next {
  width: 100vw;
  height: 100vh;
  display: flex;
  align-items: center;
}

</style>
