<template>
  <section id="contact" class="contact">
    <!-- form wrapper -->
    <fvl-form class="form" method="post" :data="form" url="/create">
      <!-- Text input component -->
      <fvl-input :value.sync="form.fullname" label="Full Name" name="fullname" />

      <!-- Textarea component -->
      <fvl-textarea :value.sync="form.bio" label="Bio" name="bio" />

    </fvl-form>
    <article>
      
    </article>
  </section>
</template>

<script>
import { FvlForm, FvlInput, FvlTextarea, FvlRadio, FvlSubmit } from 'formvuelar'

export default{
  name: 'Contact',
  components: {
    FvlForm,
    FvlInput,
    FvlTextarea,
    FvlRadio,
    FvlSubmit,
  },
  data() {
    return {
      form: {
        fullname: '',
        bio: '',
        pet: ''
      }
    }
  }
}

</script>

<style lang="scss" scoped>
@import '~formvuelar/dist/formvuelar.css';

.contact {
  width: 100vw;
  height: 100vh;
  display: grid;
  grid-template-columns: 5% 35% 20% 35% 5%;
  grid-template-rows: 20% 60% 20%;
}

.form {
  grid-column: 2 / 3;
  grid-row: 2;
}

.fvl-input-label {
  @apply block uppercase tracking-wide text-grey-darker text-lg font-bold mb-2;
}

</style>

