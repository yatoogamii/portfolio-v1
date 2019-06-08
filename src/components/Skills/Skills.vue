<template>
  <section id="skills" class="skills">
    <Skill img="./github.svg" value="70" text="html" width="width: 34%"></Skill>
    <Skill img="./react.svg" value="50" text="Js" width="width: 34%"></Skill>
    <Skill img="./linux.svg" value="70" text="html" width="width: 33.33%"></Skill>
    <Skill img="./vuejs.svg" value="60" text="css" width="width: 33.33%"></Skill>
    <Skill img="./postgresql.svg" value="60" text="Js" width="width: 33.33%"></Skill>
    <Skill img="./vim.svg" value="80" text="html" width="width: 33.33%"></Skill>
    <Skill img="./nodejs.svg" value="70" text="css" width="width: 33.33%"></Skill>
    <Skill img="./mongo.svg" value="50" text="Js" width="width: 33.33%"></Skill>
  </section>
</template>

<script>
import Skill from './Skill.vue';

  export default{
    name: 'Skills',
    components: {
      Skill
    }
  }
</script>

<style scoped>

.skills {
  width: 100vw;
  height: 100vh;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
}

</style>

