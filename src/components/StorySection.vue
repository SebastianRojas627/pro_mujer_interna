<template>
  <div class="container my-4">
    <TitleComponent :title="this.title" />
    <div class="row justify-content-center align-items-center">
      <div class="col-md-5">
        <div class="embed-responsive embed-responsive-16by9 rounded">
          <iframe
            class="embed-responsive-item b4-back"
            :src="videoUrl"
            frameborder="0"
            allow="autoplay; encrypted-media"
            allowfullscreen
          ></iframe>
        </div>
      </div>
      <div class="col-md-5">
        <p class="text-muted">{{ description }}</p>
      </div>
    </div>
  </div>
</template>

<script>
import TitleComponent from "./TitleComponent.vue";
export default {
  components: {
    TitleComponent,
  },
  data() {
    return {
      title: "Historias",
      videoUrl: "https://www.youtube.com/embed/IeA7bTr64G0",
      description:
        "Gabriela alcanzó la confianza y autoestima necesaria para animarse a ir más allá y seguir creciendo en su negocio.",
    };
  },
};
</script>
