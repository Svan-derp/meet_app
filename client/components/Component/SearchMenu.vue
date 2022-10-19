<template>
  <div class="filter-menu">
    <SelectActivityCategory class="filter-item" />
    <SelectLocation class="filter-item" />
    <b-slider
      type="is-primary"
      class="filter-item"
      size="is-medium"
      :custom-formatter="(val) => val + 'km'"
      :tooltip="false"
      indicator
      :min="1"
      :max="50"
      :value="12"
    >
    </b-slider>
    <b-datepicker class="filter-item" v-model="date" inline> </b-datepicker>
    <div class="buttons">
      <b-button class="is-light"> Wis filters</b-button>
      <b-button class="is-primary"> Zoek</b-button>
    </div>
  </div>
</template>

<script>
import SelectLocation from '@/components/Base/SelectLocation.vue';
import SelectActivityCategory from '@/components/Base/SelectActivityCategory.vue';
export default {
  data() {
    return {
      date: null,
    };
  },
  components: { SelectLocation, SelectActivityCategory },
};
</script>

<style scoped>
.filter-menu {
  max-width: 40rem;
  border-radius: 24px;
  background-color: var(--secondary);
  box-shadow: 5px 5px 20px 5px rgba(0, 0, 0, 0.4);
}
.filter-item {
  padding: 24px 16px 0px 16px;
}
.buttons {
  padding: 10px;
  justify-content: center;
}
</style>
