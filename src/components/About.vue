<template>
  <div class="container mt-4 ">
    <div class="jumbotron-fluid bg beautify">
      <div class="d-flex align-items-center justify-content-between mb-3">
        <span class="text-light lead display-4 pl-3">About Me</span>
        <img src="@/assets/gare.png" class="rounded img-fluid w-25" />
      </div>
      <div class="container">
        <p class="text-light lead">{{ p1 }}</p>
        <p class="text-light lead">{{ p2 }}</p>
        <p class="text-light lead">{{ p3 }}</p>
        <p class="text-light lead">{{ p4 }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      p1:
        "Hi, I'm Garrett.",
      p2:
        "I am passionate about problem solving and coding. I love being able to create and fix things, both functionally and aesthetically.",
      p3:
        "Over the past few years I have built, developed and maintained several websites. Head over to my Portfolio to check them out and my github if you'd like to look under the hood.",
      p4:
        "From building sites that nurture communities, I’ve learned how to lead multiple teams of people, moderators, broadcasting talent, and manage users. But most importantly, I learned getting things done and staying within deadlines and scope is paramount.",
    };
  },
};
</script>

<style scoped>
.bg {
  background-color: #27222a;
}
.portrait {
}
.beautify {
  -webkit-background-clip: border;

  background-image: linear-gradient(rgba(39, 34, 42, 0.7), rgba(39, 34, 42, 1)),
    url(../assets/aurora.jpg);
  background-size: cover;
  font-weight: 700;
}
</style>
