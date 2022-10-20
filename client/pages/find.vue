<template>
  <div class="find-page">
    <MapBox />
    <div class="columns">
      <div class="column left-area">
        <SearchMenu />
      </div>
      <div class="column right-area">
        <ListEvent />
      </div>
    </div>
  </div>
</template>

<script>
import SearchMenu from '@/components/Component/SearchMenu.vue';
<<<<<<< HEAD
import ListEvent from '@/components/Layout/ListEvents.vue';
import MapBox from '@client/components/Base/MapBox.vue';
=======
import EventList from '@/components/Layout/EventList.vue';
import MapBox from '@/components/Base/MapBox.vue';
>>>>>>> dev

export default {
  name: 'FindPage',
  components: { SearchMenu, ListEvent, MapBox },
};
</script>

<style scoped>
.left-area {
  padding: 35px 12px 0px 35px;
  max-width: 460px;
}
.right-area {
  padding: 40px 40px 40px 40px;
}
.find-page {
  margin-top: 24px;
}
</style>
