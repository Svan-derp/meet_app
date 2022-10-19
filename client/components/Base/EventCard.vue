<template>
  <div class="panel">
    <section>
      <b-collapse
        aria-id="contentIdForA11y2"
        class="panel"
        animation="slide"
        v-model="isOpen"
      >
        <template #trigger>
          <div class="panel-image"></div>
          <div
            class="panel-heading"
            aria-controls="contentIdForA11y2"
            :aria-expanded="isOpen"
          >
            <div class="columns">
              <div class="column is-half">Event title Lorum</div>
              <div class="column">address</div>
              <div class="column">09:00 - 13:30</div>
            </div>
          </div>
        </template>
        Evenement beschrijving komt hier te staan
        <footer class="card-footer">
          <a class="card-footer-item">Evenement</a>
          <a class="card-footer-item">Contact</a>
          <a class="card-footer-item">Aanmelden</a>
        </footer>
      </b-collapse>
    </section>
  </div>
</template>

<script>
export default {
  name: 'Eventcard',

  data() {
    return {
      isOpen: false,
    };
  },
};
</script>

<style scoped>
.panel {
  box-shadow: 5px 5px 20px 5px rgba(0, 0, 0, 0.2);
  border-radius: 12px;
}
.panel-image {
  height: 12rem;
  background-image: url(../../assets/pexels-pixabay-1.jpg);
  background-size: cover;
  border-radius: 12px;
}
.panel-heading {
  background-color: white;
  border-radius: 12px;
}
</style>
