<template>
  <article :style="width" class="skills__skill">
    <div class="ldBar"
         data-type="fill"
         data-fill-dir="ltr"
         :data-img="img"
         :data-value="value"
         data-img-size="125,125"
         style="margin:auto"
         data-fill-background-extrude="1"
         data-fill-background="#3D3D3D"
         ></div>
  </article>
</template>

<script>
export default{
  name: 'Skill',
  props: ['value', 'color', 'text', 'width', 'img']
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

