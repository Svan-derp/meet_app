<template>
  <div>
    <h1>HELLO from index page</h1>
    <UserList />
  </div>
</template>

<script lang="ts">
import UserList from '@/components/TestComp.vue';

export default {
  components: { UserList },
};
</script>
