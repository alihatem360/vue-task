<template>
  <div class="subheader">
    <div class="subheader__links">
      <router-link
        v-for="tab in tabs"
        :key="tab.name"
        :to="tab.path"
        class="subheader__link"
        active-class="subheader__link--active"
        exact
      >
        {{ tab.name }}
      </router-link>
    </div>
  </div>
</template>

<script>
export default {
  name: "subheader-component",
  components: {},
  data() {
    return {
      tabs: [
        { name: "Web Design", path: "/webdesign" },
        { name: "Mobile App Design", path: "/mobileappdesign" },
        { name: "Freebies", path: "/freebies" },
      ],
    };
  },
};
</script>
