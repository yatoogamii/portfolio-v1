<template>
  <article :style="width" class="skills__skill">
    <v-tooltip bottom>
      <template v-slot:activator="{ on }">
        <div class="ldBar"
             data-type="fill"
             data-fill-dir="ltr"
             :data-img="img"
             :data-value="value"
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
  props: ['value', 'width', 'img', 'title', 'tooltip'],
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

