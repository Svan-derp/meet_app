<template lang="vue">
<b-field class="quicksearch-bar">
  <SelectActivityCategory/>
  <SelectLocation />
  <NuxtLink to="/find">
    <b-button label="Zoek" type="is-primary" />
  </NuxtLink>
</b-field>
</template>

<script lang="ts">
import SelectActivityCategory from '@/components/Base/SelectActivityCategory.vue';
import SelectLocation from '@/components/Base/SelectLocation.vue';

// TODO: get compontent data and send to activity page

export default {
  name: 'QuickSearch',
  components: { SelectActivityCategory, SelectLocation },
};
</script>

<style>
.quicksearch-bar {
  box-shadow: 5px 5px 20px 15px rgba(0, 0, 0, 0.3);
}
/* .select.is-fullwidth {
  TODO: scoped is not working properly
  width: 250px;
  margin-right: -250px;
} */
</style>
