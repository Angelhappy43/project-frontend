<template>
  <div class="navbar--main fxbx">
    <div class="navbar--brand fxbx f1 headline">
      <h1>ROOST</h1>
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

};
</script>

<style scoped>
.navbar--main {
  height: 4rem;
  border-bottom: 3px solid var(--dark-acc);
  padding: .5rem 1rem;
}
.headline {
  color: var(--text-hl);
}
</style>
