<template>
  <section class="managed-cameras-top" id="managedCamerasTopSection">
    <ImageLoader v-if="loading" />
    <div class="container">
      <div class="managed-cameras-top-wrapper">
        <h1 class="text-white"> Managed Cameras</h1>
        <p class="text-white managed-cameras-top-text">Oversight and management of security cameras and access systems, enhancing safety and surveillance for businesses.</p>
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
    const section = document.getElementById('managedCamerasTopSection');
    const backgroundImage = new Image();
    backgroundImage.src = "/images/services/manag-cam-hero.webp";
    backgroundImage.onload = () => {
      section.classList.add('managed-cameras-top-image-loaded');
      this.loading = false;
    };
    backgroundImage.onerror = () => {
      section.classList.add('managed-cameras-top-image-loaded');
      this.loading = false;
    };
  },
}
</script>
<style>
.managed-cameras-top {
  position: relative;
  background-image: url("/images/services/manag-cam-hero.webp");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  background-color: #dedede;
  height: 490px;
}
.managed-cameras-top-text {
  font-size: 21px;
}
.managed-cameras-top-image-loaded {
  background-image: url("/images/services/manag-cam-hero.webp");
}
.managed-cameras-top-wrapper {
  display: flex;
  flex-direction: column;
  align-items: start;
  justify-content: start;
  gap: 31px;
  height: 100%;
}
</style>
