<template>
  <!-- footer -->
  <div>
    <div class="footer">
      <div class="footer__logo">Let's Connect</div>
      <div class="footer__links">
        <img src="../../assets/icons/Instagram.svg" alt="Instagram" />
        <img src="../../assets/icons/youtube.svg" alt="Youtube" />
        <img src="../../assets/icons/kora.svg" alt="Kora" />
      </div>

      <div class="footer__top" @click="scrollToTop">
        <p>Back to Top</p>
        <img src="../../assets/icons/short_up.svg" alt="Back to Top" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "footer-component",
  components: {},
  methods: {
    scrollToTop() {
      window.scrollTo({
        top: 0,
        behavior: "smooth",
      });
    },
  },
};
</script>
