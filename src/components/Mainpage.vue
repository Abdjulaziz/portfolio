<template>
  <About />
  <Projects />
</template>

<script>
import About from './About.vue';
import Projects from './Projects.vue';
export default {
  name: 'Mainpage',
  components: {
    About,
    Projects,
  },
};
</script>

<style lang="scss" scoped></style>
