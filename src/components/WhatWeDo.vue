<template>
  <div class="container mt-5 mb-5">
    <h1 class="text-center">¿QUÉ HACEMOS?</h1>
    <div class="row justify-content-center mt-5">
      <div class="col-md-4">
        <div class="card mb-4">
          <img
            src="../assets/card1.png"
            :alt="card1.imageAlt"
            class="card-img-top img-thumbnail custom-img"
          />
          <div class="card-body">
            <p class="card-text">{{ card1.description }}</p>
          </div>
        </div>
      </div>
      <div class="col-md-4">
        <div class="card mb-4">
          <img
            src="../assets/card2.png"
            :alt="card2.imageAlt"
            class="card-img-top img-thumbnail custom-img"
          />
          <div class="card-body">
            <p class="card-text">{{ card2.description }}</p>
          </div>
        </div>
      </div>
    </div>
    <div class="row justify-content-center mt-4">
      <div class="col-md-4">
        <div class="card mb-4">
          <img
            src="../assets/card3.png"
            :alt="card3.imageAlt"
            class="card-img-top custom-img"
          />
          <div class="card-body">
            <p class="card-text">{{ card3.description }}</p>
          </div>
        </div>
      </div>
      <div class="col-md-4">
        <div class="card mb-4">
          <img
            src="../assets/card4.png"
            :alt="card4.imageAlt"
            class="card-img-top custom-img"
          />
          <div class="card-body">
            <p class="card-text">{{ card4.description }}</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      card1: {
        imageSrc: "../assets/card1.png",
        imageAlt: "Image 1",
        description: "Salud y Bienestar",
      },
      card2: {
        imageSrc: "../assets/card1.png",
        imageAlt: "Image 2",
        description: "Apoyo Financiero",
      },
      card3: {
        imageSrc: "../assets/card1.png",
        imageAlt: "Image 3",
        description: "Capacitacion",
      },
      card4: {
        imageSrc: "../assets/card1.png",
        imageAlt: "Image 4",
        description: "Emprendimiento",
      },
    };
  },
};
</script>

<style scoped>
.custom-img {
  /* Set the desired maximum height */ /* Adjust how the image fits within the container */
  height: 10%;
  width: auto;
}
</style>
