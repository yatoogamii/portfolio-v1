<template>
  <!-- form wrapper -->
  <fvl-form class="form" method="post" :data="form" url="/create">
    <!-- Text input component -->
    <fvl-input :value.sync="form.fullname" label="Nom complet" name="nomcomplet" required />
      <!-- Text input component -->
      <fvl-input :value.sync="form.email" label="Email" name="email" type="email" required />
        <!-- Text input component -->
        <fvl-select
          label="Object"
          name="object"
          placeholder="-- sujet de votre demande --"
          :allowEmpty="true"
          :options="{ 'Professionnel': 'Professionnel', 'Bug': 'Report Bug', 'Autre': 'Autre' }"
          :selected.sync="form.object"
          />

          <!-- Textarea component -->
          <fvl-textarea :rows="5" :value.sync="form.message" label="Message" name="message" required />

            <v-btn
              :loading="loading"
              :disabled="loading"
              color="secondary"
              dark
              large
              @click="loader = 'loading'; sendMessage()"
              >
              Valider</v-btn>
            <v-btn large dark @click="resetForm">reset</v-btn>

  </fvl-form>
</template>

<script>
import { FvlForm, FvlInput, FvlTextarea, FvlSelect} from 'formvuelar';

export default{
  name: 'Form',
  components: {
    FvlForm,
    FvlInput,
    FvlTextarea,
    FvlSelect,
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
    },
    sendMessage() {
    Email.send({
    Host : "smtp.elasticemail.com",
    Username : "bracaval.elias.pro@gmail.com",
    Password : "f0d91566-4f07-4ca8-b0f3-45762dd0e933",
    To : 'bracaval.elias.pro@gmail.com',
    From : this.form.email,
    Subject : this.form.object,
    Body : this.form.message
}).then(
  message => alert(message)
);
    }
  }
}
</script>

<style lang="scss" scoped>
@import '~formvuelar/dist/formvuelar.css';

.form {
  grid-column: 2 / 3;
  grid-row: 2;
}
</style>

