<template>
  <div class="container mt-4">
    <div class="jumbotron-fluid bg">
      <div class="align-items-center justify-content-center mb-3">
        <p class="text-light lead display-4">Skills</p>
        <ul class="list-group list listBorder">
          <li
            v-for="skill in skills"
            :key="skill.id"
            class="list-group-item list border-info"
          >
            {{ skill }}
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      skills: [
        "HTML5/CSS",
        "JavaScript",
        "Vue",
        "Bootstrap",
        "Communication/Public Speaking",
        "Photoshop/GIMP",
      ],
    };
  },
};
</script>

<style scoped>
.list {
  background-color: transparent;
  color: white;
  border-color: transparent;
}
.listBorder {
  -webkit-background-clip: border;

  background-image: linear-gradient(rgba(39, 34, 42, 0.8), rgba(39, 34, 42, 1)),
    url(../assets/aurora.jpg);
  background-size: cover;
  font-weight: 700;
}
</style>
