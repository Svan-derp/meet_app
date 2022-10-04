<template lang="vue">
  <b-navbar type="is-light">
    <!-- TODO: hover and active must only underline item + ?!cursor? -->
    <template #brand>
      <NuxtLink to="/">
        <b-navbar-item>
          <!-- <img
          src="https://raw.githubusercontent.com/buefy/buefy/dev/static/img/buefy-logo.png"
          alt="Lightweight UI components for Vue.js based on Bulma"
          height="64"
          width="192"
        /> -->
          <strong>MEET_APP</strong>
        </b-navbar-item></NuxtLink
      >
    </template>
    <template #start>
      <NuxtLink to="/find"
        ><b-navbar-item> Zoek activiteit </b-navbar-item></NuxtLink
      >
      <NuxtLink to="/host">
        <b-navbar-item> Plaats activiteit</b-navbar-item>
      </NuxtLink>
      <b-navbar-dropdown label="Met ons">
        <NuxtLink to="/team"><b-navbar-item> Team </b-navbar-item></NuxtLink>
        <NuxtLink to="/contact">
          <b-navbar-item>Contact</b-navbar-item></NuxtLink
        >
        <b-navbar-item> Meld een probleem </b-navbar-item>
      </b-navbar-dropdown>
    </template>

    <template #end>
      <b-navbar-item tag="div">
        <div class="buttons">
          <NuxtLink to="/">
          <a class="button is-primary">
            <strong>Inschrijven</strong>
          </a></NuxtLink>
          <NuxtLink to="/">
          <a class="button is-light"> Aanmelden </a></NuxtLink>
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
