<template>
  <About />
  <Projects />
  <Contact />
</template>

<script>
import About from './About.vue';
import Projects from './Projects.vue';
import Contact from './Contact.vue';
export default {
  name: 'Mainpage',
  components: {
    About,
    Projects,
    Contact,
  },
};
</script>

<style lang="scss" scoped></style>
