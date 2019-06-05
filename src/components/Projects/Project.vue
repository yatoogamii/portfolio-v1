<template>
  <article class="container-project">
    <div :style="textalign" class="div-project">
      <slot name="img"></slot>
      <slot name="text"></slot>
      <slot name="tag"></slot>
      <div class="div-project__button">
        <v-btn left class="project__button" left color="#fff">Go</v-btn>
      </div>
    </div>
  </article>
</template>

<script>
export default{
  name: 'Project',
  props: ['width', 'textalign']
}
</script>

<style lang="scss" scoped>

.container-project {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100%;
  height: 100%;
}

.div-project {
  width: 100%;
  height: 100%;
  background-color: #1d1d1d;
  color: white;
  display: grid;
  grid-template-columns: 10% 80% 10%;
  grid-template-rows: 5% 50% 10% 20% 5% 10%;
  transition: all 0.5s ease;

  img {
    width: 100%;
    height: 100%;
    grid-column: 1 / 4;
    grid-row: 2 / 3;
    object-fit: cover;
    object-position: center;
  }

  h1 {
    width: 100%;
    font-size: 3rem;
    grid-column: 2 / 3;
    grid-row: 3 / 4;
  }

  .div-project__desc {
    width: 100%;
    font-size: 1.5rem;
    grid-column: 2 / 3;
    grid-row: 4 / 5;
  }

  .div-project__tag {
    grid-column: 2 / 3;
    grid-row: 5 / 6;
  }

  .div-project__button {
    width: 100%;
    grid-column: 2 / 3;
    grid-row: 6 / 7;

    .project__button {
      width: 15rem;
      height: 4rem;
      margin: auto;
      left: 0;
      right: 0;
    }
  }

  .text--red {
    color: red;
  }

}

</style>

