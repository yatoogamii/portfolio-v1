<template>
  <article :style="width" class="skills__skill">
    <div class="ldBar label-center"
         data-type="fill"
         data-fill-dir="ltr"
         :data-img="img"
         :data-value="value"
         data-img-size="150,150"
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

.ldBar-label:after {
  content: "USD";
  color: #aaa;
  margin-left: 5px;
  font-family: courier new;
  font-size: 0.7em;
  font-weight: 200;
}

</style>

