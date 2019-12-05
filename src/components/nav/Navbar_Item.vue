<template>
  <div class="navbar--item fxbx spc-ctr pointer">
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
};
</script>

<style scoped>
.navbar--item {
  width: 6rem;
}
</style>
