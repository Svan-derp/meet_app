<template>
  <div class="container">
    <div class="screen">
      <b-tabs v-model="activeStep">
        <b-tab-item label="1. Account aanmaken "> <RegisterUser /> </b-tab-item>

        <b-tab-item label="2. Voorkeuren aangeven ">
          Select categories with checkbox/cards in grid (like pinterest)
        </b-tab-item>
        <b-tab-item label="3. Acitviteiten zoeken ">
          select a filter selection and forward to find page with
          that</b-tab-item
        ></b-tabs
      >
    </div>
  </div>
</template>

<script>
import RegisterUser from '@/components/Component/RegisterUser.vue';
export default {
  components: { RegisterUser },
  data() {
    return {
      activeStep: 0,
    };
  },
  created() {
    // this.$nuxt.$on('emitRegister', ($event) => this.submitRegister($event));
  },
  methods: {
    async submitRegister(e) {
      this.activeStep + 1;
      return console.log(JSON.stringify(this.registerForm));
    },
  },
};
</script>

<style scoped>
.container {
  display: flex;
  align-items: center;
  justify-content: center;
  min-height: 800px;
}

.screen {
  position: relative;
  width: 80vw;
  border-radius: 16px;
  box-shadow: 0px 8px 24px var(--primary);
}
</style>
