<template>
  <div>
    <NavBar />
    <nuxt />
    <!-- TODO: make sure all notifications are called from here -->
  </div>
</template>

<script lang="ts">
import NavBar from '@/components/navbar.vue';

export default {
  name: 'MasterLayout',
  components: { NavBar },
};
</script>
