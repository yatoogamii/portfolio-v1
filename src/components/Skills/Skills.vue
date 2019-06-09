<template>
  <section id="skills" class="skills">
    <Skill title="Github" tooltip="Commit, PR" img="./github.svg" value="70" width="width: 34%">
    </Skill>
    <Skill title="CSS" tooltip="Flexbox, Grid, SASS"  img="./css.svg" value="80" width="width: 34%">
    </Skill>
    <Skill title="Linux" tooltip="Manjaro, Ubuntu"  img="./linux.svg" value="70" width="width: 33.33%">
    </Skill>
    <Skill title="VueJS" tooltip="Vue CLI, Nuxt.js, Vuetify" img="./vuejs.svg" value="60" width="width: 33.33%">
    </Skill>
    <Skill title="ReactJS" tooltip="RCA, Reactify" img="./react.svg" value="50" width="width: 33.33%">
    </Skill>
    <Skill title="Vim" tooltip="Plugin, Macro" img="./vim.svg" value="80" width="width: 33.33%">
    </Skill>
    <Skill title="JS/Node.js" tooltip="ES6+, Express, Mongoose, Sequelize" img="./nodejs.svg" value="70" width="width: 33.33%">
    </Skill>
    <Skill title="PostgreSQL" tooltip="Jointure" img="./postgresql.svg" value="60" width="width: 33.33%">
    </Skill>
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

