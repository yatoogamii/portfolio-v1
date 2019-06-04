<template>
  <section id="project" class="project">
    <Project width="width: 40%"></Project>
    <Project width="width: 40%"></Project>
    <Project width="width: 33.33%"></Project>
    <Project width="width: 33.33%"></Project>
    <Project width="width: 33.33%"></Project>
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

<style scoped>
.project {
  width: 100vw;
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: space-around;
  flex-wrap: wrap;
}

</style>

