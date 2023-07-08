<template>
  <div class="home">
    <Headr />
    <SubHeader />
    <ProjectList />
    <ProjectSubscribe />
    <Footer />
  </div>
</template>

<script>
import Headr from "../components/project/Headr.vue";
import SubHeader from "../components/project/SubHeader.vue";
import ProjectList from "../components/project/ProjectList.vue";
import ProjectSubscribe from "../components/project/ProjectSubscribe.vue";
import Footer from "../components/utils/Footer.vue";
export default {
  name: "HomeView",
  components: {
    Headr,
    SubHeader,
    ProjectList,
    ProjectSubscribe,
    Footer,
  },
};
</script>
