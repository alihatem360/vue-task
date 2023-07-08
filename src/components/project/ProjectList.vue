<template>
  <div class="project-list">
    <ProjectItem
      v-for="project in projects"
      :key="project.name"
      :project="project"
    />
  </div>
</template>

<script>
import ProjectItem from "./ProjectItem.vue";
export default {
  name: "ProjectList",
  components: {
    ProjectItem,
  },
  data() {
    return {
      projects: [
        {
          name: "Minify - Web Design",
          image: "/minify.svg",
        },
        {
          name: "Ant - Personal Portofolio",
          image: "/ant-personal.svg",
        },
        {
          name: "Lumy - Dashboard UI Kit",
          image: "/lumy.svg",
        },
        {
          name: "Keeper - Soccer Site",
          image: "/keeper.svg",
        },
      ],
    };
  },
};
</script>
