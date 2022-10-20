<template lang="vue">
  <div>
    <div class="columns">
      <div class="column">
        <b-field class="is-name" label="Voornaam">
          <b-input v-model="registerForm.surename"></b-input>
        </b-field>
      </div>
      <div class="column is-one-quarter">
        <b-field class="is-name" label="Tussenvoegsel">
          <b-input v-model="registerForm.namefix"></b-input>
        </b-field>
      </div>
      <div class="column">
        <b-field class="is-name" label="Achternaam">
          <b-input v-model="registerForm.lastname"></b-input>
        </b-field>
      </div>
    </div>

    <b-field label="Gebruikersnaam">
      <b-input v-model="registerForm.username"></b-input>
    </b-field>

    <b-field label="Plaats">
      <SelectLocation />
    </b-field>

    <b-field label="Email">
      <b-input type="email" v-model="registerForm.email"> </b-input>
    </b-field>

    <b-field label="Wachtwoord">
      <b-input type="password" v-model="registerForm.password" password-reveal>
      </b-input>
    </b-field>
    <b-checkbox v-model="registerForm.agreed" class="field">
      Ik ga akkoord met de gebruikersvoorwaarden
    </b-checkbox>
      <!-- @click="$nuxt.$emit('emitRegister', registerForm)" -->
    <b-button
      class="button is-primary"
      >Geef je voorkeuren aan</b-button
    >
  </div>
</template>

<script>
import SelectLocation from '@/components/Base/SelectLocation.vue';
export default {
  components: { SelectLocation },
  data() {
    return {
      name: 'John Silver',
      registerForm: {
        surename: 'John',
        namefix: 'v/d',
        lastname: 'voluit',
        email: 'email',
        username: 'john f do',
        password: 'johndeer',
      },
    };
  },
};
</script>

<style scoped>
.screen {
  position: relative;
  width: 80vw;
  border-radius: 16px;
  box-shadow: 0px 8px 24px var(--primary);
}
.columns {
  padding: 8px 5vw 0px;
}

.field:not(.is-name) {
  padding: 0px 5vw 4px;
}
.checkbox {
  margin: 16px 8px 24px 0px;
}
.button {
  margin-top: 0px;
  width: stretch;
}
</style>
