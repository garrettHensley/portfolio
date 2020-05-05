<template>
  <div class="home">
    <HelloWorld />
    <AppHolder />
    <About />
    <Skills />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";
import AppHolder from "@/components/AppHolder.vue";
import About from '@/components/About.vue';
import Skills from '@/components/Skills.vue';

export default {
  name: "Home",
  components: {
    HelloWorld,
    AppHolder,
    About,
    Skills
  },
};
</script>
