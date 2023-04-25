<template>
  <div>
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark fixed-top">
      <button class="navbar" type="button" @click="toggleMenu">
        <span class="navbar-toggler-icon"></span>
      </button>
      
      <div class="col collapse navbar-collapse">
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
      
      <div v-if="menuOpen" class="menu" style="z-index: 999;">
        <ul class="list-group">
          <li class="list-group-item"><a href="#">Menu item 1</a></li>
          <li class="list-group-item"><a href="#">Menu item 2</a></li>
          <li class="list-group-item"><a href="#">Menu item 3</a></li>
        </ul>
      </div>

      <div class="col fixed-right">
        <ul class="list-group list-unstyled">
          <li class="nav-item">
            <div class="row">
              <div class="col-sm-12">
                <small>First row of text</small>
              </div>
            </div>
          </li>
          <li class="nav-item">
            <div class="row">
              <div class="col-sm-12">
                <small>Second row of text</small>
              </div>
            </div>
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
      menuOpen: false
    }
  },
  methods: {
    toggleMenu() {
      this.menuOpen = !this.menuOpen;
    }
  }
}
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
