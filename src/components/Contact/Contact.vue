<template>
  <section id="contact" class="contact">
    <Form></Form>
    <Coordonate></Coordonate>
  </section>
</template>

<script>
import Form from './Form.vue';
import Coordonate from './Coordonate.vue';

export default{
  name: 'Contact',
  components: {
    Form,
    Coordonate
  },
}

</script>

<style lang="scss" scoped>

.contact {
  width: 100vw;
  height: 100vh;
  display: grid;
  grid-template-columns: 5% 35% 20% 35% 5%;
  grid-template-rows: 20% 60% 20%;
}

</style>

