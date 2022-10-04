<template>
  <div>
    <p class="mb-4 day-title">Vandaag</p>
    <EventCard />
    <EventCard />
    <hr class="rounded mt-6 mx-6" />
    <p class="mb-4 day-title">Morgen</p>
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
.day-title {
  font-size: x-large;
}
hr.rounded {
  border-top: 2px solid rgba(187, 187, 187, 0.1);
}
.card {
  margin-bottom: 3vh;
}
</style>
