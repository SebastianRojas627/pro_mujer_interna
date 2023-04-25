<template>
    <div class="row">
      <div class="col-md-6">
        <h1>{{ title }}</h1>
      </div>
      <div class="col-md-6">
        <p>{{ paragraph }}</p>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'TextComponent',
    data() {
      return {
        title: "POR UNA BOLIVIA DONDE TODAS LAS MUJERES PROSPEREN",
        paragraph: "Desde hace más de 30 años apoyamos a mujeres para que alcancen su máximo potencial. Pro Mujer brinda inclusión financiera y digital, capacitaciones y servicios de salud y bienestar a bajo costo.",
      };
    },
  };
  </script>
  
  <style scoped>
  h1 {
    font-size: 3rem;
    font-weight: bold;
  }
  </style>