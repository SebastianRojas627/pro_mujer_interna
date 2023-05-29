<template>
  <div>
    <h1 class="informes-title">{{ title }}</h1>
    <div class="informes-section">
      <h2 class="informes-subtitle informes-left">{{ subtitle1 }}</h2>
      <ul class="informes-list">
        <li class="informes-list-item">Sample text 1</li>
        <li class="informes-list-item">Sample text 2</li>
        <li class="informes-list-item">Sample text 3</li>
      </ul>
    </div>
    <div class="informes-section">
      <h2 class="informes-subtitle informes-left">{{ subtitle2 }}</h2>
      <ul class="informes-list">
        <li class="informes-list-item">Sample text 4</li>
        <li class="informes-list-item">Sample text 5</li>
        <li class="informes-list-item">Sample text 6</li>
      </ul>
    </div>
    <div class="informes-section">
      <h2 class="informes-subtitle informes-left">{{ subtitle3 }}</h2>
      <ul class="informes-list">
        <li class="informes-list-item">Sample text 7</li>
        <li class="informes-list-item">Sample text 8</li>
        <li class="informes-list-item">Sample text 9</li>
      </ul>
    </div>
  </div>
</template>

<style>
.informes-title {
  text-align: center;
  color: red;
  font-size: 42px;
  margin-bottom: 20px;
}

.informes-subtitle {
  text-align: left;
  color: red;
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
</style>

<script>
export default {
  name: "InformeS",
  data() {
    return {
      title: "Avisos",
      subtitle1: "Subtitle 1",
      subtitle2: "Subtitle 2",
      subtitle3: "Subtitle 3",
    };
  },
};
</script>
