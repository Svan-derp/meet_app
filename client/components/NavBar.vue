<template lang="vue">
  <b-navbar type="is-light">
    //TODO: hover and active must only underline item + ?!cursor?
    <template #brand>
      <NuxtLink class="navbar-item brand" to="/">
          <!-- <img
          src="https://raw.githubusercontent.com/buefy/buefy/dev/static/img/buefy-logo.png"
          alt="Lightweight UI components for Vue.js based on Bulma"
          height="64"
          width="192"
        /> -->
          <strong>MEET_APP</strong>
        </NuxtLink
      >
    </template>
    <template #start>
      <NuxtLink class="navbar-item" to="/find"> Zoek activiteit </NuxtLink>
      <NuxtLink class="navbar-item" to="/host"> Plaats activiteit </NuxtLink>
      <b-navbar-dropdown label="Met ons">
        <NuxtLink class="navbar-item" to="/team"> Team </NuxtLink>
        <NuxtLink class="navbar-item" to="/contact">
          Contact</NuxtLink
        >
         <b-navbar-item> Meld een probleem </b-navbar-item>
      </b-navbar-dropdown>
    </template>

    <template #end>
        <div class="buttons">
          <NuxtLink to="/">
          <a class="button is-primary">
            <strong>Inschrijven</strong>
          </a></NuxtLink>
          <NuxtLink to="/">
          <a class="button is-light"> Aanmelden </a></NuxtLink>
        </div>
      
    </template>
  </b-navbar>
</template>

<script lang="ts">
import { Component, Vue } from 'nuxt-property-decorator';

@Component
export default class MenuHeader extends Vue { }
</script>

<style lang="scss" scoped>
.navbar-start {
  padding-left: 15vw !important;
}

.button {
  margin-right: 20px
}

// TODO: work on this glued stuff (exclude brand focus+hover and dropdown bgcolor)
a.navbar-item:focus {
  background-color: var(--secondary) !important;
}
a.navbar-item:hover {
  background-color: var(--secondary) !important;
  border-bottom: 3px solid var(--primary) !important;
}
a.navbar-item.nuxt-link-exact-active:not(.brand) {
  border-bottom: 5px solid var(--primary) !important;
}
</style>
