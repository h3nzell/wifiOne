<template>
  <section class="managed-media-wall-top" id="managedMediaWallTopSection">
    <ImageLoader v-if="loading" />
    <div class="container">
      <div class="managed-media-wall-top-wrapper">
        <h1 class="text-white">Managed Media Wall</h1>
        <p class="text-white managed-media-wall-top-text">Professional management of media walls and signage, delivering dynamic content for effective communication and branding.</p>
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
    const section = document.getElementById('managedMediaWallTopSection');
    const backgroundImage = new Image();
    backgroundImage.src = "/images/services/managed-media-wall-hero.webp";
    backgroundImage.onload = () => {
      section.classList.add('managed-media-wall-top-image-loaded');
      this.loading = false;
    };
    backgroundImage.onerror = () => {
      section.classList.add('managed-media-wall-top-image-loaded');
      this.loading = false;
    };
  },
}
</script>
<style>
.managed-media-wall-top {
  position: relative;
  background-image: url("/images/services/managed-media-wall-hero.webp");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  background-color: #dedede;
  height: 490px;
}
.managed-media-wall-top-text {
  font-size: 21px;
}
.managed-media-wall-top-image-loaded {
  background-image: url("/images/services/managed-media-wall-hero.webp");
}
.managed-media-wall-top-wrapper {
  display: flex;
  flex-direction: column;
  align-items: start;
  justify-content: start;
  gap: 31px;
  height: 100%;
}
</style>
