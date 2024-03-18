<template>
  <section class="about-us-top" id="aboutUsTopSection">
    <ImageLoader v-if="loading" />
      <div class="container">
        <div class="about-us-top-wrapper">
          <h1 class="text-white about-us-top-title">About Us</h1>
          <p class="text-white about-us-top-text">Beyond Connectivity: Get to Know WifiOne – Your Trusted Partner in Transformative Network Solutions.</p>
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
  name:'BreadCrump',
  components: {ImageLoader},
  data() {
    return {
      loading: true,
    };
  },
  mounted() {
    const section = document.getElementById('aboutUsTopSection');
    const backgroundImage = new Image();
    backgroundImage.src = "/images/about-us/hero.webp";
    backgroundImage.onload = () => {
      section.classList.add('about-us-top-image-loaded');
      this.loading = false;

    };
    backgroundImage.onerror = () => {
      section.classList.add('about-us-top-image-loaded');
      this.loading = false;
    };
  },
}
</script>
<style>
  .about-us-top {
    background-image: url("/images/about-us/hero.webp");
    position: relative;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    background-color: #dedede;
  }
  .about-us-top-text {
    font-size: 21px;
  }
  .about-us-top-image-loaded {
    background-image: url("../../assets/images/about-us/hero.webp");
  }
  .about-us-top-wrapper {
    display: flex;
    flex-direction: column;
    align-items: start;
    justify-content: start;
    gap: 31px;
    height: 100%;
  }
</style>
