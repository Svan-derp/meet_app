<<<<<<< HEAD
<template lang="vue">
<div>
    <NavBar />
    <Nuxt />
=======
<template>
  <div>
    <NavBar />
    <nuxt />
>>>>>>> demo
    <!-- TODO: make sure all notifications are called from here -->
  </div>
</template>

<script lang="ts">
import NavBar from '@/components/Component/navbar.vue';

export default {
  name: 'MasterLayout',
  components: { NavBar },
};
</script>

<style></style>
