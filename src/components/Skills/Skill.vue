<template>
  <article :style="width" class="skills__skill">
    <v-tooltip bottom>
      <template v-slot:activator="{ on }">
        <div :class="allClass"
             data-type="fill"
             data-fill-dir="ltr"
             :data-img="img"
             :data-value="pourcent"
             data-img-size="125,125"
             style="margin:auto"
             v-on="on"
             data-fill-background-extrude="1"
             data-fill-background="#3D3D3D"
             ></div>
      </template>
      <span> 
        <h1>{{ title }}</h1>
        <p>{{ tooltip }}</p>
      </span>
    </v-tooltip>
  </article>
</template>

<script>
export default{
  name: 'Skill',
  props: ['value', 'width', 'img', 'title', 'tooltip', 'theme'],
  data() {
    return {
      allClass: "ldBar " + this.theme,
      pourcent: 0
    };
  },
  mounted() {
    setTimeout(() => { 
      const github = document.getElementsByClassName('github')[0].ldBar;
      const css = document.getElementsByClassName('css')[0].ldBar;
      const linux = document.getElementsByClassName('linux')[0].ldBar;
      const vim = document.getElementsByClassName('vim')[0].ldBar;
      const react = document.getElementsByClassName('react')[0].ldBar;
      const vuejs = document.getElementsByClassName('vuejs')[0].ldBar;
      const postgresql = document.getElementsByClassName('postgresql')[0].ldBar;
      const js = document.getElementsByClassName('js')[0].ldBar;
      github.set(0)
      github.set(70)
      css.set(0)
      css.set(80)
      linux.set(0)
      linux.set(70)
      vim.set(0)
      vim.set(80)
      react.set(0)
      react.set(50)
      vuejs.set(0)
      vuejs.set(60)
      js.set(0)
      js.set(70)
      postgresql.set(0)
      postgresql.set(60)
    }, 700);
  }
  
}

</script>

<style lang="scss" scoped>

.skills__skill {
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 1.3rem;
  height: 33.33%;
}
</style>

