<template>
  <section id="avisos">
    <div class="bg-light pt-3">
      <TitleComponent :title="this.title" />
      <div class="informes-section">
        <h2 class="informes-subtitle informes-left">{{ subtitle1 }}</h2>
        <ul class="informes-list">
          <li class="informes-list-item">
            <a class="informes-link" href="https://example.com/document1.pdf"
              >Convocatoria De Licitación Pública Para Contratación De Seguro
              Colectivo</a
            >
          </li>
          <li class="informes-list-item">
            <a class="informes-link" href="https://example.com/document2.pdf"
              >Condiciones Particulares - Seguro de desgravamen Hipotecario
              2023-2026</a
            >
          </li>
          <li class="informes-list-item">
            <a class="informes-link" href="https://example.com/document3.pdf"
              >Resultados de la Licitación Pública del Seguro de desgravamen
              N°001/2023</a
            >
          </li>
        </ul>
      </div>
      <div class="informes-section">
        <h2 class="informes-subtitle informes-left">{{ subtitle2 }}</h2>
        <ul class="informes-list">
          <li class="informes-list-item">
            <a class="informes-link" href="https://example.com/document4.pdf"
              >Calificación de Desempeño en RSE 2020</a
            >
          </li>
          <li class="informes-list-item">
            <a class="informes-link" href="https://example.com/document5.pdf"
              >Coeficiente de Adecuación Patrimonial (CAP) noviembre 2019</a
            >
          </li>
          <li class="informes-list-item">
            <a class="informes-link" href="https://example.com/document6.pdf"
              >Coeficiente de Adecuación Patrimonial (CAP) 2019 y 2020</a
            >
          </li>
        </ul>
      </div>
      <div class="informes-section">
        <h2 class="informes-subtitle informes-left">{{ subtitle3 }}</h2>
        <ul class="informes-list">
          <li class="informes-list-item">
            <a class="informes-link" href="https://example.com/document7.pdf"
              >Seguro Plan Tranquilidad</a
            >
          </li>
          <li class="informes-list-item">
            <a class="informes-link" href="https://example.com/document8.pdf"
              >Seguro Vida + Salud Preventiva</a
            >
          </li>
          <li class="informes-list-item">
            <a class="informes-link" href="https://example.com/document9.pdf"
              >Seguro de Vida por Covid - 19</a
            >
          </li>
        </ul>
      </div>
    </div>
  </section>
</template>

<style>
.informes-title {
  text-align: center;
  color: green;
  font-size: 42px;
  margin-bottom: 20px;
}

.informes-subtitle {
  text-align: left;
  color: rgb(22, 132, 0);
  font-size: 24px;
  margin-top: 30px;
  margin-left: 30px;
}

.informes-section {
  margin-bottom: 30px;
}

.informes-list {
  list-style-type: none;
  padding-left: 0;
  margin-top: 10px;
}

.informes-list-item {
  margin-left: 30px;
  margin-bottom: 5px;
}

.informes-link {
  color: inherit;
  text-decoration: none;
}

.informes-link:hover {
  text-decoration: underline;
}
</style>

<script>
import TitleComponent from "./TitleComponent.vue";
export default {
  components: {
    TitleComponent,
  },

  name: "InformeS",
  data() {
    return {
      title: "Avisos",
      subtitle1:
        "CONVOCATORIA DE LICITACIÓN PÚBLICA PARA CONTRATACIÓN DE SEGURO COLECTIVO",
      subtitle2: "INFORMACIÓN ADICIONAL",
      subtitle3: "SEGUROS EN PRO MUJER",
    };
  },
};
</script>
