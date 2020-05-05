<template>
  <div class="container">
    <div
      class="jumbotron text-light"
      :style="{
        backgroundImage:
          'linear-gradient(rgba(39, 34, 42, 1), rgba(39, 34, 42, .2)), url(' +
          img +
          ')',
      }"
    >
      <h1 class="display-5">{{ name }}</h1>
      <p class="lead text-light">
        {{ description }}
      </p>

      <a
        class="btn btn-primary test btn-lg"
        :href="source"
        target="_blank"
        role="button"
        >Source</a
      >
    </div>
  </div>
</template>

<script>
export default {
  props: {
    name: {
      type: String,
      required: true,
    },
    img: String,
    source: String,
    description: String,
  },
};
</script>

<style scoped>
.bg {
  background-image: linear-gradient(red, yellow, blue);
}
.test {
  -webkit-text-fill-color: rgba(39, 34, 42, 1);
  -webkit-background-clip: border-box;

  background-image: url(../assets/aurora.jpg);
  background-size: cover;
  font-weight: 700;
}
</style>
