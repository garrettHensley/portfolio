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
        "Hello, I'm Garrett Hensley. Ever since I can remember I've been interested in technology. From my first Gameboy, to my first PC built, to my first PHP program written in highschool, to the first website I've created. Technology and it's inner-workings have always been a passion of mine.",
      p2:
        "Over the past few years I have built, developed and maintained several websites. Brainscans.net, I created to serve as an inclusive environment for people of all skill levels to engage in competitive gaming. Because I believe everyone deserves a shot at testing their mettle. And Underlords.pro, originally an off-shoot of Brainscans.net, serving today as one of the largest competitive hubs for Valve’s video game Dota Underlords.",
      p3:
        "I’ve learned a great deal from creating these organizations. I’ve learned how to lead multiple teams of people, moderators, broadcasting talent, and players. But most importantly, I learned to just get things done when necessary. Like making tough decisions on the spot, or implementing new website features.",
      p4:
        "I am passionate about problem solving and coding. Doing these things brings me much joy and fulfillment in life. I love being able to create and fix things, on the functionality side and the aesthetic side.",
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
