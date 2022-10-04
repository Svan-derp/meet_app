<template lang="vue">
<b-field>
  <SelectActivityCategory />
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
