<template>
  <div class="container pt-5 pb-5">
    <div class="row">
      <div class="col-md-6">
        <h1 class="display-6">{{ title }}</h1>
      </div>
      <div class="col-md-6">
        <p class="lead">{{ description }}</p>
      </div>
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
    };
  },
};
</script>
