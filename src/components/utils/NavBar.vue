<template>
  <div class="nav-bar">
    <div class="nav-bar__logo">LOGO</div>
    <div class="nav-bar__links">
      <router-link
        v-for="tab in tabs"
        :key="tab.name"
        :to="tab.path"
        class="nav-bar__link"
        active-class="nav-bar__link--active"
        exact
      >
        {{ tab.name }}
      </router-link>
    </div>
  </div>
</template>

<script>
export default {
  name: "NavBar",
  components: {},
  data() {
    return {
      tabs: [
        { name: "Home", path: "/" },
        { name: "About", path: "/about" },
        { name: "Project", path: "/project" },
        { name: "Contact", path: "/contact" },
      ],
    };
  },
};
</script>
