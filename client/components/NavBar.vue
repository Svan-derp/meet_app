<template>
  <b-navbar type="is-light">
    <!-- TODO: hover and active must only underline item + ?!cursor? -->
    <template #brand>
      <b-navbar-item
        ><NuxtLink to="/">
          <!-- <img
          src="https://raw.githubusercontent.com/buefy/buefy/dev/static/img/buefy-logo.png"
          alt="Lightweight UI components for Vue.js based on Bulma"
          height="64"
          width="192"
        /> -->
          <strong>MEET_APP</strong>
        </NuxtLink>
      </b-navbar-item>
    </template>
    <template #start>
      <b-navbar-item>
        <NuxtLink to="/find">Zoek activiteit </NuxtLink></b-navbar-item
      >
      <b-navbar-item>
        <NuxtLink to="/host">Plaats activiteit </NuxtLink></b-navbar-item
      >
      <b-navbar-dropdown label="Met ons">
        <b-navbar-item><NuxtLink to="/team"> Team </NuxtLink></b-navbar-item>
        <b-navbar-item
          ><NuxtLink to="/contact"> Contact</NuxtLink></b-navbar-item
        >
        <b-navbar-item> Meld een probleem </b-navbar-item>
      </b-navbar-dropdown>
    </template>

    <template #end>
      <b-navbar-item tag="div">
        <div class="buttons">
          <a class="button is-primary">
            <strong>Inschrijven</strong>
          </a>
          <a class="button is-light"> Aanmelden </a>
        </div>
      </b-navbar-item>
    </template>
  </b-navbar>
</template>

<script lang="ts">
import { Component, Vue } from 'nuxt-property-decorator';

@Component
export default class MenuHeader extends Vue {}
</script>

<style lang="scss">
.navbar-start {
  padding-left: 10vw;
}
</style>
