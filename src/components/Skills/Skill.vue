<template>
  <article :style="width" class="skills__skill">
    <v-progress-circular
      :rotate="360"
      :size="130"
      :width="17"
      :value="value"
      :color="color"
      >
      {{ this.text }}
    </v-progress-circular>

  </article>
</template>

<script>
export default{
  name: 'Skill',
  props: ['value', 'color', 'text', 'width']
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

