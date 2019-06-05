<template>
  <section id="contact" class="contact">
    <!-- form wrapper -->
    <fvl-form class="form" method="post" :data="form" url="/create">
      <!-- Text input component -->
      <fvl-input :value.sync="form.fullname" label="Nom complet" name="nomcomplet" required="true" />
        <!-- Text input component -->
        <fvl-input :value.sync="form.email" label="Email" name="email" type="email" required="true" />
          <!-- Text input component -->
          <fvl-select
            label="Object"
            name="object"
            placeholder="-- sujet de votre demande --"
            :allowEmpty="true"
            :options="{ 'Professionnelle': 'Professionnelle', 'Bug': 'Report Bug', 'Autre': 'Autre' }"
            :selected.sync="form.object"
            />

            <!-- Textarea component -->
            <fvl-textarea rows="5" :value.sync="form.message" label="Message" name="message" required="true"/>

              <v-btn
                :loading="loading"
                :disabled="loading"
                color="secondary"
                dark
                large
                @click="loader = 'loading'"
                >
                Valider</v-btn>
              <v-btn large dark @click="resetForm">reset</v-btn>

    </fvl-form>
    <article>

    </article>
  </section>
</template>

<script>
import { FvlForm, FvlInput, FvlTextarea, FvlSelect} from 'formvuelar'

export default{
  name: 'Contact',
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

</style>

