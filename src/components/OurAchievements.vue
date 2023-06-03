<template>
  <div class="container">
    <h2 class="text-center">{{ title }}</h2>
    <div class="row">
      <div class="col">
        <div class="text-center">
          <div class="card-body">
            <h1 class="text-primary">{{ number1 }}</h1>
            <p class="text-muted">{{ description1 }}</p>
          </div>
        </div>
      </div>
      <div class="col">
        <div class="text-center">
          <div class="card-body">
            <h1 class="text-primary">{{ number2 }}</h1>
            <p class="text-muted">{{ description2 }}</p>
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
      title: "EN MÁS DE 30 AÑOS:",
      number1: "$4.4MM",
      description1: "Desembolsamos US $4,4 milmillones en créditos",
      number2: "+10M",
      description2: "Brindamos más de 10 millones de servicios de salud",
    };
  },
};
</script>

<style scoped>
.container {
  margin-top: 50px;
}
</style>
