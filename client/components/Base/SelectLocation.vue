<template>
  <b-autocomplete
    :data="['Amsterdam', 'Utrecht', 'Amersfoort']"
    placeholder="Locatie"
    icon="map-marker"
    expanded
    clearable
    @select="(option) => (selected = option)"
  >
    <template #empty>No results found</template>
  </b-autocomplete>
</template>
<script lang="ts"></script>
