<template>
  <div class="container">
    <div class="row">
      <div class="col-md-6">
        <h1 class="display-6">{{ title }}</h1>
      </div>
      <div class="col-md-6">
        <p class="lead">{{ description }}</p>
      </div>
    </div>
    <div class="pt-4">
      <h1 class="text-center display-6">{{ subHeader }}</h1>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      title: "POR UNA BOLIVIA DONDE TODAS LAS MUJERES PROSPEREN",
      description:
        "Desde hace más de 30 años apoyamos a mujeres para que alcancen su máximo potencial. Pro Mujer brinda inclusión financiera y digital, capacitaciones y servicios de salud y bienestar a bajo costo.",
      subHeader: "SÉ PARTE DE ESTA GRAN COMUNIDAD. ¡EMPIEZA HOY!",
    };
  },
};
</script>
