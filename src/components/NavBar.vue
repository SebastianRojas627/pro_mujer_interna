<template>
  <nav
    class="navbar navbar-expand-md navbar-dark bg-dark fixed-top"
    style="height: 85px"
    :class="{ transparent: isTransparent }"
  >
    <a class="navbar-brand" href="#inicio">
      <img
        src="../assets/bank-logo-example.png"
        alt="Logo"
        width="auto"
        height="40"
        class="m-3"
      />
    </a>

    <div class="collapse navbar-collapse" id="navbarNav">
      <ul class="navbar-nav mr-auto">
        <li class="nav-item">
          <a class="nav-link text-white" href="#inicio">Inicio</a>
        </li>
        <li class="nav-item">
          <a class="nav-link text-white" href="#quehacemos">Que Hacemos</a>
        </li>
        <li class="nav-item">
          <a class="nav-link text-white" href="#quienessomos">Quienes Somos</a>
        </li>
        <li class="nav-item">
          <a class="nav-link text-white" href="#ubicaciones">Ubicaciones</a>
        </li>
        <li class="nav-item">
          <a class="nav-link text-white" href="#avisos">Avisos</a>
        </li>
        <li class="nav-item">
          <a class="nav-link text-white" href="#informacion">Informacion</a>
        </li>
      </ul>
    </div>
    <a
      href="https://wa.me/59165165908"
      target="_blank"
      class="navbar-text m-3 d-flex justify-content-end text-white"
    >
      <img
        src="../assets/WhatsApp-Logo.wine.png"
        alt="WhatsApp"
        width="auto"
        height="55"
      />
    </a>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      isTransparent: true,
    };
  },
  mounted() {
    window.addEventListener("scroll", this.handleScroll);
  },
  beforeUnmount() {
    window.removeEventListener("scroll", this.handleScroll);
  },
  methods: {
    handleScroll() {
      this.isTransparent = window.pageYOffset === 0;
    },
  },
};
</script>

<style scoped>
.navbar {
  background-color: rgba(0, 0, 0, 0.85) !important;
  transition: background-color 0.3s ease;
}

.transparent {
  background-color: transparent !important;
}

.text-white {
  color: white !important;
}

.text-black {
  color: black !important;
}
</style>
