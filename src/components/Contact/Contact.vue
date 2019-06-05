<template>
  <section id="contact" class="contact">
    <Form></Form>
  </section>
</template>

<script>
import Form from './Form.vue';

export default{
  name: 'Contact',
components: {
    Form
  },
  data() {
    return {
      form: {
        fullname: '',
        email: '',
        object: '',
        message: '',
      },
      loader: null,
      loading: false
    }
  },
  watch: {
    loader() {
      const l = this.loader
      console.log(this);
      console.log(this[l]);
      this[l] = !this[l]

      setTimeout(() => (this[l] = false), 2000)

      this.loader = null
    }
  },
  methods: {
    resetForm() {
      this.form.fullname = '';
      this.form.email = '';
      this.form.object = '';
      this.form.message = '';
    }
  }
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

