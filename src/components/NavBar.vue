<template>
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark m-auto fixed-top m-3" style="height: 85px;" :class="{'transparent': isTransparent}">
    <a class="navbar-brand" href="#">
      <img
        src="('bank-logo-example.png')"
        alt="Logo"
        width="auto"
        height="40"
      />
    </a>
    <div class="collapse navbar-collapse" id="navbarNav">
      <ul class="navbar-nav mr-auto">
        <li class="nav-item">
          <a :class="{'text-white': isTransparent, 'text-black': !isTransparent}" class="nav-link" href="#">Home</a>
        </li>
        <li class="nav-item">
          <a :class="{'text-white': isTransparent, 'text-black': !isTransparent}" class="nav-link" href="#">About</a>
        </li>
        <li class="nav-item">
          <a :class="{'text-white': isTransparent, 'text-black': !isTransparent}" class="nav-link" href="#">Services</a>
        </li>
        <li class="nav-item">
          <a :class="{'text-white': isTransparent, 'text-black': !isTransparent}" class="nav-link" href="#">Contact</a>
        </li>
      </ul>
    </div>
    <a href="https://wa.me/59165165908" target="_blank" class="navbar-text m-3">
      <img
        src="../assets/WhatsApp-Logo.wine.png"
        alt="WhatsApp"
        width="auto"
        height="55"
      />
      <p :class="{'text-white': isTransparent, 'text-black': !isTransparent}" class="nav-item">¿Necesitas Ayuda?</p>
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
    window.addEventListener('scroll', this.handleScroll);
  },
  beforeUnmount() {
    window.removeEventListener('scroll', this.handleScroll);
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
  background-color: rgba(169, 169, 169, 0.5) !important;
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
