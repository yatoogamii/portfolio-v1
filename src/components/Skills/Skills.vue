<template>
  <section id="skills" class="skills">
    <Skill color="blue" value="90" text="html" width="width: 34%"></Skill>
    <Skill color="green" value="70" text="Js" width="width: 34%"></Skill>
    <Skill color="blue" value="90" text="html" width="width: 33.33%"></Skill>
    <Skill color="red" value="50" text="css" width="width: 33.33%"></Skill>
    <Skill color="green" value="70" text="Js" width="width: 33.33%"></Skill>
    <Skill color="blue" value="90" text="html" width="width: 33.33%"></Skill>
    <Skill color="red" value="50" text="css" width="width: 33.33%"></Skill>
    <Skill color="green" value="70" text="Js" width="width: 33.33%"></Skill>
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

