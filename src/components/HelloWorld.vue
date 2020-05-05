<template>
  <div class="container">
    <div class="jumbotron bg">
      <p class="display-4 text-light">Hi, I'm</p>
      <h1 class="display-3 knockout weight">Garrett Hensley</h1>
      <p class="text-light lead mt-4">Web Developer</p>
      <p class="text-light">JS | HTML | CSS | Vue</p>
      <div class="d-flex justify-content-start">
        <a
          class="btn aurora btn-info btn-lg mr-1"
          href="mailto:garrettmichaelhensley@gmail.com"
          role="button"
          >Contact</a
        >
        <a
          class="btn aurora btn-info btn-lg mx-1"
          href="http://garretthensley.me/resume.html"
          target="_blank"
          role="button"
          >Resume</a
        >
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.knockout {
  -webkit-text-fill-color: transparent;
  -webkit-background-clip: text;

  background-image: url(../assets/aurora.jpg);
  color: white;
  padding-bottom: 0.1em;
}

.bg {
  /*
    background-color: #27222A;
    */
  background-color: transparent;
}
.weight {
  font-weight: normal;
}
jumbotron {
  border-radius: 0;
}
.aurora {
  -webkit-text-fill-color: rgba(39, 34, 42, 1);
  -webkit-background-clip: border-box;

  background-image: url(../assets/aurora.jpg);
  background-size: cover;
  font-weight: 700;
}
</style>
