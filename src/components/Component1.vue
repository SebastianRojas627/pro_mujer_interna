<template>
    <div class="row">
      <div class="col-sm-3 col-md-3 mb-4" v-for="(image, index) in images" :key="index">
        <div class="card">
          <img :src="image.src" class="card-img-top" :alt="image.alt">
          <div class="card-body">
            <p class="card-text">{{ image.description }}</p>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
  name: 'Component',
    data() {
      return {
        images: [
          {
            src: "https://via.placeholder.com/300x200",
            alt: "Image 1",
            description: "Description of image 1",
          },
          {
            src: "https://via.placeholder.com/300x200",
            alt: "Image 2",
            description: "Description of image 2",
          },
          {
            src: "https://via.placeholder.com/300x200",
            alt: "Image 3",
            description: "Description of image 3",
          },
          {
            src: "https://via.placeholder.com/300x200",
            alt: "Image 4",
            description: "Description of image 4",
          },
        ],
      };
    },
  };
  </script>
  
  <style scoped>
  .card {
    border: 1px solid #ccc;
    border-radius: 4px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  }
  .card-img-top {
    height: 200px;
    object-fit: cover;
    border-radius: 4px 4px 0 0;
  }
  </style>
  