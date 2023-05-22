<template>
  <div class="position-relative mb-5">
    <img class="img-fluid" src="../assets/background1.jpg" alt="Image Cover" />
    <div class="position-absolute bottom-0 start-0 p-3 text-white text-center">
      <h2>{{ imageText }}</h2>
      <p>{{ imageSubtext }}</p>
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
.container-fluid {
  padding: 0;
  margin: 0;
}
.col {
  padding: 0;
  margin: 0;
}
.img-fluid {
  width: 100%;
}
</style>
