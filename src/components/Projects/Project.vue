<template>
    <article :style="width">
      <div class="container-project">
        <img src="https://media-cdn.tripadvisor.com/media/photo-s/09/2b/37/3c/ocean-blue-tenerife.jpg" alt="preview site"/>
      </div>
    </article>
</template>

<script>
export default{
  name: 'Project',
  props: ['width']
}
</script>

<style lang="scss" scoped>

.container-project {
  background-color: red;
  width: 50%;
}

img {
  width: 100%;
  height: 50%;
}

</style>

