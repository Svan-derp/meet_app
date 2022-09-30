<template>
  <div>
    <h1>fetch component:</h1>
    <b-button @click="getUsers()">refresh</b-button>
    <ul class="user-list">
      <li v-for="user in users" :key="user.id">
        <span>{{ user.name }}</span>
      </li>
    </ul>
  </div>
</template>

<script lang="ts">
import { User } from '@common/UserInterface';
import { Component, Vue } from 'nuxt-property-decorator';

@Component
export default class UserList extends Vue {
  users: User[] = [];
  loading = false;

  async getUsers() {
    return this.fetchUsers();
  }

  async fetchUsers() {
    try {
      this.loading = true;

      this.users = (await this.$axios.get('users'))?.data ?? [];
    } finally {
      this.loading = false;
    }
  }
}
</script>

<style></style>
