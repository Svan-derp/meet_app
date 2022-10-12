<template>
  <div class="find-page">
    <MapBox />
    <div class="columns">
      <div class="column left-area">
        <SearchMenu />
      </div>
      <div class="column right-area">
        <EventList />
      </div>
    </div>
  </div>
</template>

<script>
import SearchMenu from '@/components/Component/SearchMenu.vue';
import EventList from '@/components/Layout/FindEventsList.vue';
import MapBox from '@/components/Base/MapBox.vue';

export default {
  name: 'FindPage',
  components: { SearchMenu, EventList, MapBox },
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
.find-page {
  margin-top: 24px;
  background-color: rgba(0, 0, 0, 0.01);
}
</style>
