<template>
  <section id="project" class="project">
    <Project>
    <template v-slot:img>
      <img src="https://media-cdn.tripadvisor.com/media/photo-s/09/2b/37/3c/ocean-blue-tenerife.jpg" alt="preview site"/>
    </template>
    <template v-slot:text>
      <h1>test 1</h1>
      <p class="div-project__desc">Ipsum enim sunt nesciunt minus id Ratione similique minus dolor nobis commodi Nisi tenetur similique?</p>
      <p class="div-project__tag text--red">#HTML #CSS #JS</p>
    </template>
    </Project>
    <Project textalign="text-align: right">
    <template v-slot:img>
      <img src="https://media-cdn.tripadvisor.com/media/photo-s/09/2b/37/3c/ocean-blue-tenerife.jpg" alt="preview site"/>
    </template>
    <template v-slot:text>
      <h1>test 2</h1>
      <p class="div-project__desc">Ipsum enim sunt nesciunt minus id Ratione similique minus dolor nobis commodi Nisi tenetur similique?</p>
      <p class="div-project__tag text--red">#HTML #CSS #JS</p>
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
