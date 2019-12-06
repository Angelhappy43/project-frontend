<template>
  <div class="dashboard view fxbx f1 spc-ctr">

    <img
      v-if="this.imageSource"
      :src="this.imageSource" alt=""
    />
    <h3 
      v-else
      class="no-image-text"
    >
      Currently no images received... please check back.
    </h3>
  </div>
</template>

<script>
export default {
  data() {
    return {
      imageSource: '',
    };
  },
};
</script>

<style scoped>
.no-image-text {
  color: var(--bright-acc)
}
</style>
