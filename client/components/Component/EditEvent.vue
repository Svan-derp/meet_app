<template>
  <div>
    <b-field label="Evenementnaam">
      <b-input v-model="EventForm.name"></b-input>
    </b-field>

    <b-field label="Categorie">
      <SelectActivityCategory />
    </b-field>

    <b-field label="Plaats">
      <SelectLocation />
    </b-field>

    <b-field label="Beschrijving">
      <b-input type="email" v-model="EventForm.description"> </b-input>
    </b-field>
    <b-field>
      <b-button @click="submitRegister()" class="button is-primary"
        >Aanmaken</b-button
      >
    </b-field>
  </div>
</template>

<script>
import SelectActivityCategory from '@/components/Base/SelectActivityCategory.vue';
import SelectLocation from '@/components/Base/SelectLocation.vue';

export default {
  components: { SelectActivityCategory, SelectLocation },
  data() {
    return {
      name: 'John Silver',
      EventForm: {
        name: 'John',
        catergory: 'v/d',
        location: 'voluit',
        description: 'geef een korte beschrijving',
      },
    };
  },
  methods: {
    submitRegister() {
      return console.log(JSON.stringify(this.registerForm));
    },
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
