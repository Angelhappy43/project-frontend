<template>
  <div class="welcome view fxbx f1">
    <div class="hero fxbx spc-ctr fd-c f4">
      <h1 class="hero-title">Welcome to the ROOST Interface</h1>
      <p class="tagline">The bestest low-levelest Raspberry Pi security camera!</p>
      <div class="buttons">
        <button
          @click="$router.push('/dashboard')"
          class="btn goto-dash"
          >View Dashboard!
        </button>
        <button
          class="btn"
          >View on Github
        </button>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  name: 'home',
};
</script>

<style scoped>
.hero-title {
  margin: 1rem 0;
}
.tagline {
  color: var(--text-hl)
}
.goto-dash {
  margin-top: 5rem;
  margin-right: 2rem;
}
</style>
