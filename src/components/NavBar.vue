<template>
  <div>
    <nav
      class="navbar navbar-expand-lg navbar-dark bg-dark fixed-top pt-3 pb-3"
    >
      <div class="navbar-brand" href="#">
        <img
          src="../assets/bank-logo-example.png"
          width="auto"
          height="35"
          alt="Logo banco"
        />
      </div>

      <div class="collapse navbar-collapse ml-auto">
        <ul class="navbar-nav">
          <li class="nav-item active">
            <a class="nav-link" href="#">Home</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">About</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Contact</a>
          </li>
        </ul>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  data() {
    return {
      menuOpen: false,
    };
  },
  methods: {
    toggleMenu() {
      this.menuOpen = !this.menuOpen;
    },
  },
};
</script>

<style>
.menu {
  position: absolute;
  top: 56px;
  left: 0;
  width: 200px;
  background-color: #fff;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.3);
  padding: 10px;
}

.menu ul {
  margin: 0;
  padding: 0;
}

.menu li {
  margin: 0;
  padding: 0;
  list-style: none;
}

.menu a {
  display: block;
  padding: 5px;
  color: #333;
}

.menu a:hover {
  background-color: #eee;
}
</style>
