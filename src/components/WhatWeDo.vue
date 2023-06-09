<template>
  <div class="pt-5 pb-5">
    <div class="container">
      <h1 class="text-center">¿QUÉ HACEMOS?</h1>
      <div class="row justify-content-center mt-5">
        <div class="col-md-4">
          <div class="card-wrapper">
            <div class="card mb-4">
              <div class="img-wrapper">
                <img
                  :src="card1.imageSrc"
                  :alt="card1.imageAlt"
                  class="card-img-top custom-img"
                />
                <div class="img-overlay"></div>
                <div class="card-hover-text">
                  <p>{{ card1.hoverText }}</p>
                </div>
              </div>
              <div class="card-body">
                <p class="card-text bigger-text">{{ card1.description }}</p>
              </div>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="card-wrapper">
            <div class="card mb-4">
              <div class="img-wrapper">
                <img
                  :src="card2.imageSrc"
                  :alt="card2.imageAlt"
                  class="card-img-top custom-img"
                />
                <div class="img-overlay"></div>
                <div class="card-hover-text">
                  <p>{{ card2.hoverText }}</p>
                </div>
              </div>
              <div class="card-body">
                <p class="card-text bigger-text">{{ card2.description }}</p>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="row justify-content-center mt-4">
        <div class="col-md-4">
          <div class="card-wrapper">
            <div class="card mb-4">
              <div class="img-wrapper">
                <img
                  :src="card3.imageSrc"
                  :alt="card3.imageAlt"
                  class="card-img-top custom-img"
                />
                <div class="img-overlay"></div>
                <div class="card-hover-text">
                  <p>{{ card3.hoverText }}</p>
                </div>
              </div>
              <div class="card-body">
                <p class="card-text bigger-text">{{ card3.description }}</p>
              </div>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="card-wrapper">
            <div class="card mb-4">
              <div class="img-wrapper">
                <img
                  :src="card4.imageSrc"
                  :alt="card4.imageAlt"
                  class="card-img-top custom-img"
                />
                <div class="img-overlay"></div>
                <div class="card-hover-text">
                  <p>{{ card4.hoverText }}</p>
                </div>
              </div>
              <div class="card-body">
                <p class="card-text bigger-text">{{ card4.description }}</p>
              </div>
            </div>
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
        imageSrc: require("../assets/card1.png"),
        imageAlt: "Image 1",
        description: "Salud y Bienestar",
        hoverText:
          "Ofrecemos servicios de salud a bajo costo, entre ellos: mamografías, tamizajes, consultas médicas y telemedicina.",
      },
      card2: {
        imageSrc: require("../assets/card2.png"),
        imageAlt: "Image 2",
        description: "Apoyo Financiero",
        hoverText:
          "Brindamos apoyo financiero para tu autonomía económica a través de distintas modalidades que se adaptan a sus necesidades: créditos individuales y grupales.",
      },
      card3: {
        imageSrc: require("../assets/card3.png"),
        imageAlt: "Image 3",
        description: "Capacitacion",
        hoverText:
          "Impartimos cursos, talleres y capacitaciones para que puedas desarrollar habilidades y destrezas que te aporten independencia.",
      },
      card4: {
        imageSrc: require("../assets/card4.png"),
        imageAlt: "Image 4",
        description: "Emprendimiento",
        hoverText:
          "A través de Pro Mujer puedes aprender a impulsar tu negocio o a generarlo desde cero. Con herramientas como Emprende promujer. ",
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
  border-radius: 10px; /* Añadido el borde curvo */
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
  border-radius: 10px;
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
  color: #0099ff;
  text-align: center;
  font-weight: bold;
  font-size: 20px;
}

.bigger-text {
  font-size: 24px;
  color: #0099ff;
  font-weight: bold;
}
</style>
