<template>
  <div>
    <h1 class="informes-title">{{ title }}</h1>
    <div class="row">
      <div class="col-md-4">
        <div class="informes-section">
          <h2 class="informes-subtitle informes-left">{{ subtitle1 }}</h2>
          <ul>
            <li>Sample text 1</li>
            <li>Sample text 2</li>
            <li>Sample text 3</li>
          </ul>
        </div>
      </div>
      <div class="col-md-4">
        <div class="informes-section">
          <h2 class="informes-subtitle informes-left">{{ subtitle2 }}</h2>
          <ul>
            <li>Sample text 4</li>
            <li>Sample text 5</li>
            <li>Sample text 6</li>
          </ul>
        </div>
      </div>
      <div class="col-md-4">
        <div class="informes-section">
          <h2 class="informes-subtitle informes-left">{{ subtitle3 }}</h2>
          <ul>
            <li>Sample text 7</li>
            <li>Sample text 8</li>
            <li>Sample text 9</li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
.informes-title {
  text-align: center;
  color: red;
  font-size: 40px;
}

.informes-subtitle {
  text-align: left;
  color: #555;
  font-size: 18px;
  margin-top: 10px;
}

.informes-left {
  margin-left: 20px;
}

.informes-section {
  margin-bottom: 20px;
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
