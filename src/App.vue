<template>
  <div id="app" class=" fxbx fd-c">
    <Navbar />
    <img src="./assets/color-chart.png" alt="">
    <router-view/>
  </div>
</template>

<script>
import Navbar from './components/nav/Navbar_Main.vue';

export default {
  components: {
    Navbar,
  },
};
</script>

<style>
@import url('./assets/css/flexbox-utility.css');
@import url('./assets/css/main.css');

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  /* color: #42b983; */
}
</style>
