<template>
  <div class="position-relative mb-5">
    <img class="img-fluid" src="../assets/background1.jpg" alt="Image Cover" />
    <div class="position-absolute bottom-0 start-0 p-3 text-white text-center" style="margin-top: -1rem;">
      <h2 class="display-2">{{ imageText }}</h2>
      <p class="display-5">{{ imageSubtext }}</p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      imageText: "30+",
      imageSubtext: "Creando oportunidades para mujeres",
    };
  },
};
</script>

<style scoped>
.img-fluid {
  width: 100%;
}
</style>
