<template>
  <section id="quienessomos">
    <div class="bg-light py-5">
      <div class="container">
        <TitleComponent title="¿QUIENES SOMOS?" />
        <div class="row justify-content-center mt-5">
          <div class="col-md-4">
            <div class="card-wrapper">
              <div class="card mb-4">
                <div class="img-wrapper">
                  <img
                    src="../assets/vision.jpg"
                    :alt="card1.imageAlt"
                    class="card-img-top custom-img"
                  />
                  <div class="img-overlay"></div>
                  <div class="card-hover-text">
                    <p>{{ card1.hoverText }}</p>
                  </div>
                </div>
                <div class="card-body">
                  <p class="card-text">{{ card1.description }}</p>
                </div>
              </div>
            </div>
          </div>
          <div class="col-md-4">
            <div class="card-wrapper">
              <div class="card mb-4">
                <div class="img-wrapper">
                  <img
                    src="../assets/mision.png"
                    :alt="card2.imageAlt"
                    class="card-img-top custom-img"
                  />
                  <div class="img-overlay"></div>
                  <div class="card-hover-text">
                    <p>{{ card2.hoverText }}</p>
                  </div>
                </div>
                <div class="card-body">
                  <p class="card-text">{{ card2.description }}</p>
                </div>
              </div>
            </div>
          </div>
          <div class="col-md-4">
            <div class="card-wrapper">
              <div class="card mb-4">
                <div class="img-wrapper">
                  <img
                    src="../assets/vision.jpg"
                    :alt="card3.imageAlt"
                    class="card-img-top custom-img"
                  />
                  <div class="img-overlay"></div>
                  <div class="card-hover-text">
                    <p>{{ card3.hoverText }}</p>
                  </div>
                </div>
                <div class="card-body">
                  <p class="card-text">{{ card3.description }}</p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import TitleComponent from "./TitleComponent.vue";
export default {
  components: {
    TitleComponent,
  },
  data() {
    return {
      card1: {
        imageSrc: require("../assets/card1.png"),
        imageAlt: "Image 1",
        description: "Visión",
        hoverText: "Una América Latina donde todas las mujeres prosperan.",
      },
      card2: {
        imageSrc: require("../assets/card2.png"),
        imageAlt: "Image 2",
        description: "Mandato",
        hoverText: "Convertirnos en una plataforma sostenible a gran escala que le proporciona recursos y herramientas relevantes y transformadoras a las mujeres de América Latina a lo largo de sus vidas.",
      },
      card3: {
        imageSrc: require("../assets/card3.png"),
        imageAlt: "Image 3",
        description: "Misión",
        hoverText: "Empoderar a mujeres de escasos recursos para que alcancen su potencial máximo.",
      },
    };
  },
};
</script>

<style scoped>
.custom-img {
  height: 100%;
  width: 100%;
  object-fit: cover;
  border-radius: 10px;
}

.img-wrapper {
  position: relative;
  overflow: hidden;
}

.img-overlay {
  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  width: 100%;
  background-color: rgba(0, 0, 0, 0.6);
  opacity: 0;
  border-radius: 40px;
  transition: opacity 0.3s ease;
}

.card-wrapper:hover .img-overlay {
  opacity: 1;
}

.card-hover-text {
  display: none;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  text-align: center;
  color: white;
  font-weight: bold;
  font-size: 18px;
}

.card-wrapper:hover .card-hover-text {
  display: block;
}

.card {
  border: none;
  border-radius: 10px;
  overflow: hidden;
}

.card-body {
  padding: 10px;
}

.card-text {
  color: #466D1D;
  text-align: center;
  font-weight: bold;
  font-size: 20px;
}
</style>
