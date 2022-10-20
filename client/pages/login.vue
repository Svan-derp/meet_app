<template>
  <div class="container">
    <div class="screen">
      <div>
        <b-field label="Email">
          <b-input type="email" v-model="email" maxlength="30"> </b-input>
        </b-field>

        <b-field label="Wachtwoord">
          <b-input type="password" v-model="password" password-reveal>
          </b-input>
        </b-field>
        <b-button @click="submitRegister()" class="button is-primary"
          >Registreer</b-button
        >
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      email: 'email',
      password: 'test',
    };
  },
  methods: {
    submitRegister() {
      return console.log(JSON.stringify(this.email + this.password));
    },
  },
};
</script>

<style scoped>
.container {
  display: flex;
  align-items: center;
  justify-content: center;
  min-height: 100vh;
}

.screen {
  position: relative;
  padding-top: 24px;
  width: 360px;
  border-radius: 16px;
  box-shadow: 0px 8px 24px var(--primary);
}

.field {
  padding: 0px 5vw 0px;
}

.button {
  margin-top: 24px;
  width: stretch;
}
</style>
