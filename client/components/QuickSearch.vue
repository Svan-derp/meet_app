<template>
  <div>
    <b-field>
      <SelectActivityCategory />
      <SelectLocation />
      <b-button label="Zoek" type="is-primary" />
    </b-field>
  </div>
</template>

<script lang="ts">
import SelectActivityCategory from '@/components/Base/SelectActivityCategory.vue';
import SelectLocation from '@/components/Base/SelectLocation.vue';

// TODO: get compontent data

export default {
  name: 'QuickSearch',
  components: { SelectActivityCategory, SelectLocation },
};
</script>
