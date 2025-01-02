<template>
  <div id="app">
    <Header />
    <About />
    <Projects />
    <Skills />
    <Contact />
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import About from "@/components/About.vue";
import Projects from "@/components/Projects.vue";
import Skills from "@/components/Skills.vue";
import Contact from "@/components/Contact.vue";

export default {
  name: "App",
  components: {
    Header,
    About,
    Projects,
    Skills,
    Contact,
  },
};
</script>

<style>
/* Tambahkan gaya global */
</style>
