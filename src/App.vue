<template>
  <div id="app" class=" fxbx fd-c">
    <Navbar />
    <router-view />
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

</style>
