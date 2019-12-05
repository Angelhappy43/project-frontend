<template>
  <div class="navbar--main fxbx f1">
    <div class="navbar--brand fxbx f1 headline">
      <h1>Simple Security Camera</h1>
    </div>
    <NavbarItem text="Welcome" />
    <NavbarItem text="Dashboard" />
  </div>
</template>

<script>
import navbarItem from './Navbar_Item.vue';

export default {
  components: {
    NavbarItem: navbarItem,
  },
  computed: {
    currentRoute() {
      return this.$router.name;
    },
  },
};
</script>

<style scoped>
.navbar--main {
  border-bottom: 3px solid var(--dark-acc);
  padding: .5rem 1rem;
}
.headline {
  color: var(--text-hl);
}
</style>
