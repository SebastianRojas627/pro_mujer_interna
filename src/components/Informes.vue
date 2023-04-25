<template>
  <div>
    <h1>{{ title }}</h1>
    <div class="row">
      <div class="md-4">
        <h2>{{ subtitle1 }}</h2>
        <ul>
          <li>Sample text 1</li>
          <li>Sample text 2</li>
          <li>Sample text 3</li>
        </ul>
      </div>
      <div class="md-4">
        <h2>{{ subtitle2 }}</h2>
        <ul>
          <li>Sample text 4</li>
          <li>Sample text 5</li>
          <li>Sample text 6</li>
        </ul>
      </div>
      <div class="md-4">
        <h2>{{ subtitle3 }}</h2>
        <ul>
          <li>Sample text 7</li>
          <li>Sample text 8</li>
          <li>Sample text 9</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
    name: 'InformeS',
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
