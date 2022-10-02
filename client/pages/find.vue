<template>
  <div class="columns">
    <div class="column left-area">
      <SearchMenu />
    </div>
    <div class="column right-area">
      <EventList />
    </div>
  </div>
</template>

<script>
import SearchMenu from '@/components/SearchMenu.vue';
import EventList from '@client/components/EventList.vue';

export default {
  name: 'FindPage',
  components: { SearchMenu, EventList },
};
</script>

<style scoped>
.left-area {
  padding-top: 35px;
  padding-left: 35px;
  max-width: 460px;
}
.right-area {
  padding: 40px;
}
</style>
