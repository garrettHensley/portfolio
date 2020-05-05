<template>
  <div class="container-fluid">
    <div
      id="carouselExampleControls"
      class="carousel slide"
      data-ride="carousel"
    >
      <div class="carousel-inner">
        <div
          v-for="(app, index) in apps"
          :key="app.id"
          :class="{ active: index == 1 }"
          class="carousel-item"
        >
          <Card
            :name="app.name"
            :description="app.description"
            :source="app.source"
            :img="app.img"
            class="WeatherVue"
          />
        </div>
      </div>
      <a
        class="carousel-control-prev"
        href="#carouselExampleControls"
        role="button"
        data-slide="prev"
      >
        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
        <span class="sr-only">Previous</span>
      </a>
      <a
        class="carousel-control-next"
        href="#carouselExampleControls"
        role="button"
        data-slide="next"
      >
        <span class="carousel-control-next-icon" aria-hidden="true"></span>
        <span class="sr-only">Next</span>
      </a>
    </div>
  </div>
</template>

<script>
import Card from "@/components/Card.vue";
import Apps from "@/assets/apps.json";

export default {
  data() {
    return {
      apps: Apps.apps,
      publicPath: process.env.BASE_URL,
    };
  },
  components: {
    Card,
  },
};
</script>

<style scoped></style>
