<template>
    <article :style="width" class="container-project">
      <div class="div-project">
        <slot name="img"></slot>
        <slot name="text"></slot>
        <div class="div-project__button">
           <v-btn small dark left color="#1d1d1d">Go</v-btn>
        </div>
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
  margin-top: 2rem;
  display: flex;
  align-items: center;
  justify-content: center;
}

.div-project {
  background-color: #fff;
  width: 50%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  transition: all 0.5s ease;

  &:hover {
    width: 55%;
  }

 .div-project__button {
    width: 100%;
  }
}

img {
  width: 100%;
  height: 50%;
}

h1 {
  padding: 0.5rem;
  width: 90%;
  text-align: left;
}

p {
  width: 90%;
  text-align: left;
}
</style>

