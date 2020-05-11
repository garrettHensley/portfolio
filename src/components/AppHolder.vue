<template>
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
      
        <Card
          v-for="app in apps"
          :key="app.id"
          :name="app.name"
          :description="app.description"
          :source="app.source"
          :img="app.img"
          class="WeatherVue"
        />
      
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
