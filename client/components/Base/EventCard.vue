<template>
  <div class="card">
    <div class="card-image">
      <figure class="top-image">
        <img
          src="https://bulma.io/images/placeholders/96x96.png"
          alt="Banne Image"
        />
      </figure>
    </div>
    <div class="card-content">
      <div class="media">
        <div class="media-content">
          <p class="title is-4">Sneak preview and roadmap reveal</p>
          <p class="subtitle is-6">@meet_app</p>
        </div>
      </div>

      <div class="content">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus nec
        iaculis mauris. <a>@bulmaio</a>. <a href="#">#css</a>
        <a href="#">#responsive</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'EventCard',
};
</script>

<style scoped>
.top-image img {
  height: 125px !important;
  width: stretch !important;
}
</style>
