<template>
  <div>
    <NavBar />
    <Nuxt />
    <!-- TODO: make sure all notifications are called from here -->
  </div>
</template>

<script lang="ts">
import NavBar from '@/components/Component/NavBar.vue';

export default {
  name: 'MasterLayout',
  components: { NavBar },
};
</script>

<style></style>
