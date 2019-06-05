<template>
  <article class="container-project">
    <div class="div-project">
      <slot name="img"></slot>
      <slot name="text"></slot>
      <slot name="tag"></slot>
      <div class="div-project__button">
        <v-btn left dark class="project__button" left color="#1d1d1d">Go</v-btn>
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
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100%;
  height: 100%;
}

.div-project {
  width: 100%;
  height: 100%;
  background-color: #fff;
  display: grid;
  grid-template-columns: 10% 80% 10%;
  grid-template-rows: 50% 10% 25% 5% 10%;
  transition: all 0.5s ease;

  img {
    width: 100%;
    height: 100%;
    grid-column: 1 / 4;
    grid-row: 1 / 2;
    object-fit: cover;
    object-position: center;
  }

  h1 {
    width: 90%;
    text-align: left;
    font-size: 3rem;
    grid-column: 2 / 3;
    grid-row: 2 / 3;
  }

  .div-project__desc {
    width: 90%;
    text-align: left;
    font-size: 1.5rem;
    grid-column: 2 / 3;
    grid-row: 3 / 4;
  }

  .div-project__tag {
    grid-column: 2 / 3;
    grid-row: 4 / 5;
  }

  .div-project__button {
    width: 100%;
    grid-column: 2 / 3;
    grid-row: 5 / 6;

    .project__button {
      width: 15rem;
      height: 4rem;
      margin-left: auto;
      left: 0;
    }
  }

}

</style>

