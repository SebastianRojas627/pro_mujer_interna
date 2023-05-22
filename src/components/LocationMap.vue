<template>
  <h1 class="mb-3">UBICACIONES</h1>
  <div class="mb-5"><div id="map"></div></div>
</template>

<script>
import L from "leaflet";
import "leaflet/dist/leaflet.css";

export default {
  mounted() {
    this.initMap();
  },
  methods: {
    initMap() {
      const map = L.map("map", {
        center: [-16.5, -68.15], // Set the initial center to La Paz, Bolivia
        zoom: 13,
      });

      L.tileLayer("https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png", {
        attribution:
          'Map data &copy; <a href="https://www.openstreetmap.org/">OpenStreetMap</a> contributors',
        maxZoom: 18,
      }).addTo(map);

      map.invalidateSize(); // Refresh the map size to ensure it takes 80% of the screen width
    },
  },
};
</script>

<style>
#map {
  height: 35rem;
  width: 90%;
  margin: auto;
}
</style>
