<template>
  <section class="service-top" id="serviceTopSection">
    <ImageLoader v-if="loading" />
    <div class="container">
      <div class="service-top-wrapper">
        <h1 class="text-white"> Services</h1>
        <p class="text-white service-top-text">From scalable connectivity solutions to proactive security measures, we deliver performance and
          <br> reliability, empowering your business operations</p>
        <div class="text-left">
          <a class="button blue-btn button-icon text-left" href="/contact-us"><span class="btn-effect"> Contact Us</span></a>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
import ImageLoader from "~/components/themes/ImageLoader.vue";

export default {
  name:'Hero',
  components: {ImageLoader},
  data() {
    return {
      loading: true,
    };
  },
  mounted() {
    const section = document.getElementById('serviceTopSection');
    const backgroundImage = new Image();
    backgroundImage.src = "/images/services/hero.webp";
    backgroundImage.onload = () => {
      section.classList.add('service-top-image-loaded');
      this.loading = false;

    };
    backgroundImage.onerror = () => {
      section.classList.add('service-top-image-loaded');
      this.loading = false;
    };
  },
}
</script>
<style>
.service-top {
  position: relative;
  background-image: url("/images/services/hero.webp");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}
.service-top-text {
  font-size: 21px;
}
.service-top-image-loaded {
  background-image: url("/images/services/hero.webp");
}
.service-top-wrapper {
  display: flex;
  flex-direction: column;
  align-items: start;
  justify-content: start;
  gap: 31px;
  height: 100%;
}
</style>
