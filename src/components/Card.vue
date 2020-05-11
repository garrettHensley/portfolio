<template>
  <div class="col mb-2">
    <div class="card text-white bg-dark">
      <img :src="img" class="img-fluid" />
      <div class="cardbody px-3">
        <h4 class="card-title">{{ name }}</h4>
        <p class="lead text-light">
          {{ description }}
        </p>
        <div class="text-center">
          <a
            class="btn btn-primary test btn-lg"
            :href="source"
            target="_blank"
            role="button"
            >Source</a
          >
        </div>
      </div>
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
