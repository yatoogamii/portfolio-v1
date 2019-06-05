<template>
  <section id="project-next" class="project-next">
    <Project>
    <template v-slot:img>
      <img src="https://media-cdn.tripadvisor.com/media/photo-s/09/2b/37/3c/ocean-blue-tenerife.jpg" alt="preview site"/>
    </template>
    <template v-slot:text>
      <h1>test 2</h1>
      <p class="div-project__desc">Ipsum enim sunt nesciunt minus id Ratione similique minus dolor nobis commodi Nisi tenetur similique?</p>
      <p class="div-project__tag text--red">#HTML #CSS #JS</p>
    </template>
    </Project>
    <Project textalign="text-align: right">
    <template v-slot:img>
      <img src="https://media-cdn.tripadvisor.com/media/photo-s/09/2b/37/3c/ocean-blue-tenerife.jpg" alt="preview site"/>
    </template>
    <template v-slot:text>
      <h1>test 3</h1>
      <p class="div-project__desc">Ipsum enim sunt nesciunt minus id Ratione similique minus dolor nobis commodi Nisi tenetur similique?</p>
      <p class="div-project__tag text--red">#HTML #CSS #JS</p>
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
