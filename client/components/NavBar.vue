<template>
  <b-navbar>
    <template #brand>
      <b-navbar-item
        ><NuxtLink to="/">
          <!-- <b-navbar-item tag="router-link" :to="{ path: '/' }"> -->
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
        <NuxtLink to="/dashboard/find"
          >Zoek activiteit
        </NuxtLink></b-navbar-item
      >
      <b-navbar-item>
        <NuxtLink to="/dashboard/host"
          >Plaats activiteit
        </NuxtLink></b-navbar-item
      >
      <b-navbar-dropdown>
        <b-navbar-item href="#"> Team </b-navbar-item>
        <b-navbar-item href="#"> Contact </b-navbar-item>
        <b-navbar-item href="#"> Meld een probleem </b-navbar-item>
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

<style>
.navbar {
  background-color: aquamarine;
}

.navbar-start {
  padding-left: 10vw;
}
</style>
