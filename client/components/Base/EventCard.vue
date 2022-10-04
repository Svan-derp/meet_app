<template>
  <div class="card">
    <div class="card-image">
      <figure class="top-image"></figure>
    </div>
    <div class="card-content">
      <p class="title is-4">Sneak preview and roadmap reveal</p>
      <div class="columns">
        <div class="column">
          <NuxtLink to="/profile[offical_meet_app]" class="subtitle is-6"
            >@official_meet_app</NuxtLink
          >
        </div>
        <div class="subtitle is-6 column">
          <p>vanaf 12:00 tot 15:00</p>
          <p>Herengracht 462, Amsterdam</p>
        </div>
      </div>
      <div class="buttons">
        <NuxtLink class="button" to="/event[event]">Meer informatie</NuxtLink>
        <NuxtLink class="button" to="/event/join[user]"
          >Direct aanmelden</NuxtLink
        >
        <NuxtLink class="button" to="/event/join[user]"
          >Direct aanmelden</NuxtLink
        >
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
.card {
  box-shadow: 5px 5px 20px 5px rgba(0, 0, 0, 0.2);
  border-radius: 12px;
}
.card:hover .card-content {
  height: 100%;
}
.top-image {
  height: 15rem;
  background-image: url(../../assets/pexels-pixabay-1.jpg);
  background-size: cover;
  border-radius: 12px;
}
.card-content {
  color: white;
  position: absolute;
  border-radius: 4px;
  bottom: 0;
  background-color: var(--primary);
  overflow: hidden;
  width: 100%;
  height: 0;
  transition: 0.6s ease;
}
.title {
  color: white;
  /* TODO: fix for mobile display */
  margin-top: -10px;
}
.subtitle {
  color: white;
}
.buttons {
  margin-top: -8px;
  padding: 16px;
  justify-content: center;
}
.button {
  width: 45%;
}
</style>
