<template>
  <section id="skills" class="skills">
    <Skill value="90" text="html" width="width: 34%"></Skill>
    <Skill value="100" text="Js" width="width: 34%"></Skill>
    <Skill value="90" text="html" width="width: 33.33%"></Skill>
    <Skill img="./vuejs.svg" value="60" text="css" width="width: 33.33%"></Skill>
    <Skill value="70" text="Js" width="width: 33.33%"></Skill>
    <Skill value="90" text="html" width="width: 33.33%"></Skill>
    <Skill img="./nodejs.svg" value="70" text="css" width="width: 33.33%"></Skill>
    <Skill value="70" text="Js" width="width: 33.33%"></Skill>
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

