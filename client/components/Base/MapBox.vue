<template>
  <div>
    <div id="map-box" />
  </div>
</template>

<script>
export default {
  data: () => ({}),
  mounted: () => {
    const mapbox = require('mapbox-gl');

    mapbox.accessToken = process.env.MAPBOX_KEY;
    const map = new mapbox.Map({
      container: 'map-box',
      style: 'mapbox://styles/mapbox/streets-v11',
      center: [5.2, 52.1], // [lon, lat]
      zoom: 8,
    });
  },
  methods: {},
};
</script>

<style>
#map-box {
  margin-top: -24px;
  height: 420px;
}
.mapboxgl-control-container .mapboxgl-ctrl-attrib {
  display: none !important;
}
</style>
