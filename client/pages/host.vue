<template>
  <div class="host-page">
    <EditEvent />
  </div>
</template>

<script>
import EditEvent from '@/components/Component/EditEvent.vue';

export default {
  name: 'HostPage',
  components: { EditEvent },
};
</script>

<style scoped>
.host-page {
  margin-top: 24px;
}
</style>
