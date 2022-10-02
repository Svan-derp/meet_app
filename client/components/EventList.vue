<template>
  <div>
    <p class="mb-4">Vandaag</p>
    <EventCard />
    <EventCard />
  </div>
</template>

<script>
import EventCard from '@/components/Base/EventCard.vue';

export default {
  components: { EventCard },
};
</script>

<style>
.card {
  margin-bottom: 3vh;
}
</style>
