<template>
  <section id="ubicaciones">
    <div class="mb-5 pt-5">
      <TitleComponent title="UBICACIONES" />
      <div id="map"></div>
    </div>
  </section>
</template>

<script>
import L from "leaflet";
import "leaflet/dist/leaflet.css";
import TitleComponent from "./TitleComponent.vue";
export default {
  components: {
    TitleComponent,
  },
  mounted() {
    this.initMap();
  },
  methods: {
    initMap() {
      const map = L.map("map", {
        center: [-16.5, -68.15],
        zoom: 13,
      });

      L.tileLayer("https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png", {
        attribution:
          'Map data &copy; <a href="https://www.openstreetmap.org/">OpenStreetMap</a> contributors',
        maxZoom: 18,
      }).addTo(map);

      map.invalidateSize();
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
