<template>
  <div>
    <h1>HELLO from index page</h1>
    <UserList />
  </div>
</template>

<style lang="scss">
.user-list {
  list-style: none;
  padding-left: 0;
}
</style>

<script lang="ts">
import UserList from '@/components/test.vue';

export default {
  components: { UserList },
};
</script>
