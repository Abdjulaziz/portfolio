<template>
  <mainpage />
</template>

<script>
import Mainpage from './components/Mainpage.vue';

export default {
  name: 'App',
  components: {
    Mainpage,
  },
};
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Arimo&display=swap');
$mainColor: #ffa500;
$secondaryColor: #035d96;

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Arimo', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  transition: 0.3s;
}
html {
  background-color: #002841;
}

/* width */
::-webkit-scrollbar {
  width: 10px;
  height: 10px;
}

/* Track */
::-webkit-scrollbar-track {
  background: #002841;
}

/* Handle */
::-webkit-scrollbar-thumb {
  background: #ffa500;
}

/* Handle on hover */
::-webkit-scrollbar-thumb:hover {
  background: #b67702;
}
</style>
