<template lang="vue">
<div>
  <section class="section is-large quote">
    <!-- TODO:Loop in over few quotes -->
    <h1 class="title">Zoek activiteiten bij jouw in de buurt!</h1>
    <h2 class="subtitle">
      Plan of neem deel aan activiteiten waar je aanmeldingen en updates kan bijhouden.
    </h2>
  </section>
  <SearchQuick class="container search-bar" />
</div>
</template>

<script lang="ts">
import SearchQuick from '@/components/Component/SearchQuick.vue';

export default {
  name: 'IndexPage',
  components: { SearchQuick },
};
</script>

<style lang="scss" scoped>
section.quote {
  background-image: url(../assets/youssef-naddam.jpg);
  background-size: cover;
}

.search-bar {
  margin-top: -22px;
  max-width: 800px;
}
</style>
