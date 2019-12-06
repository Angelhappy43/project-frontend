<template>
  <div
    @click="navigateRoute"
    v-if="this.text !== this.currentRoute"
    class="navbar--item fxbx spc-ctr pointer">
    {{ text }}
  </div>
</template>

<script>
export default {
  props: {
    text: {
      type: String,
      required: true,
    },
  },
  computed: {
    currentRoute() {
      return this.$route.name;
    },
  },
  methods: {
    navigateRoute() {
      this.$router.push(this.text.toLowerCase());
    },
  },
};
</script>

<style scoped>
.navbar--item {
  width: 6rem;
}
</style>
