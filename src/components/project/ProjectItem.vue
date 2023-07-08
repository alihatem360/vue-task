<template>
  <div class="project-item">
    <img :src="project.image" :alt="project.name" class="project-image" />
    <h2 class="project-name">{{ project.name }}</h2>
    <div class="project-links">
      <a href="#" class="project-link">
        <img src="../../assets/icons/layers.svg" alt="View Study Case" />
        <span> View Study Case </span>
      </a>
      <a href="#" class="project-link">
        <img src="../../assets/icons/show.svg" alt="Visit Website" />
        <span> Live Preview </span>
      </a>
    </div>
  </div>
</template>

<script>
export default {
  name: "ProjectItem",
  props: {
    project: {
      type: Object,
      required: true,
    },
  },
};
</script>
