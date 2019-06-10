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

            <!-- add loading in disabled props --> 
            <v-btn
              :loading="loading"
              :disabled="true"
              color="secondary"
              dark
              large
              @click="loader = 'loading'; sendMessage()"
              >
              Valider
            </v-btn>
              <v-btn disabled large dark @click="resetForm">reset</v-btn>
              <p class="doesnt-work">doesn't work yet</p>

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
      this.form.object = '-- sujet de votre demande --';
      this.form.message = '';
    },
    sendMessage() {
      setTimeout(() => {this.resetForm()}, 1000)
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
.doesnt-work {
  grid-column: 2 / 3;
  color: #d1d1d1;
  font-size: 1.5rem;
  padding: .5rem;
}
</style>

