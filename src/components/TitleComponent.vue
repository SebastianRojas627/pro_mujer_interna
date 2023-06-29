<template>
  <div class="d-flex justify-content-center">
    <h1 :class="[gradientClass, 'fw-bold', 'display-4']">{{ title }}</h1>
  </div>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      required: true,
    },
  },
  computed: {
    gradientClass() {
      return "text-gradient-green-transparent";
    },
  },
};
</script>

<style>
.text-gradient-green-transparent {
  background: linear-gradient(to right, #016601, rgba(1, 102, 1, 0.2));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
</style>
