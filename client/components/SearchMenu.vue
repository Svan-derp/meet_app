<template>
  <div class="filter-menu">
    <SelectActivityCategory class="filter-item special" />
    <SelectLocation class="filter-item narrow" />
    <b-slider
      type="is-primary"
      class="filter-item narrow"
      size="is-medium"
      :custom-formatter="(val) => val + 'km'"
      :tooltip="false"
      indicator
      :min="1"
      :max="50"
      :value="12"
    >
    </b-slider>
    <b-datepicker class="filter-item narrow" v-model="date" inline>
    </b-datepicker>
    <div class="buttons">
      <b-button class="is-light"> Wis filters</b-button>
      <b-button class="is-primary"> Zoek</b-button>
    </div>
  </div>
</template>

<script>
import SelectLocation from './Base/SelectLocation.vue';
import SelectActivityCategory from './Base/SelectActivityCategory.vue';
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
  background-color: var(--secondary);
  max-width: 400px;
  border-radius: 24px;
}
.filter-item {
  padding: 24px;
  padding-bottom: 3px;
}
.buttons {
  padding: 10px;
  justify-content: center;
}
.narrow {
  padding-top: 10px;
}
</style>
