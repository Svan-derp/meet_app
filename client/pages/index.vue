<template>
  <div>
    <section class="section is-large quote">
      <!-- TODO:Loop in over few quotes -->
      <h1 class="title">Zoek activiteiten bij jouw in de buurt!</h1>
      <h2 class="subtitle">
        Plan of neem deel aan activiteiten waar je aanmeldingen en updates kan
        bijhouden.
      </h2>
      <!--  -->
    </section>
    <QuickSearch class="container search-bar" />
  </div>
</template>

<script lang="ts">
import QuickSearch from '../components/QuickSearch.vue';

export default {
  name: 'IndexPage',
  components: { QuickSearch },
};
</script>

<style lang="scss" scoped>
section.quote {
  background-image: url(https://cdn.shortpixel.ai/spai/q_lossy+w_739+to_avif+ret_img/https://www.mindful.org/content/uploads/party.png);
  background-size: cover;
}

.search-bar {
  margin-top: -22px;
  max-width: 800px;
}
</style>
