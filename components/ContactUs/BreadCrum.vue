<template>
  <section class="contact-us-top" id="contactUsTopSection">
    <ImageLoader v-if="loading" />
      <div class="container">
        <div class="contact-us-top-wrapper">
          <h1 class="text-white contact-us-top-title"> Contact Us</h1>
          <p class="text-white contact-us-top-text">We welcome your inquiries—use the form below to get in touch.</p>
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
    const section = document.getElementById('contactUsTopSection');
    const backgroundImage = new Image();
    backgroundImage.src = "/images/contact-us/contact-us.webp";
    backgroundImage.onload = () => {
      section.classList.add('contact-us-top-image-loaded');
      this.loading = false;

    };
    backgroundImage.onerror = () => {
      section.classList.add('contact-us-top-image-loaded');
      this.loading = false;
    };
  },
}
</script>
<style>
  .contact-us-top {
    position: relative;
    background-image: url("/images/contact-us/contact-us.webp");
    background-position: center;
    background-repeat: no-repeat;
    background-size:cover;
    height: 490px;
    background-color: #dedede;
  }
  .contact-us-top-text {
    font-size: 21px;
  }
  .contact-us-top-image-loaded {
    background-image: url("/images/contact-us/contact-us.webp");
  }
  .contact-us-top-wrapper {
    display: flex;
    flex-direction: column;
    align-items: start;
    justify-content: start;
    gap: 31px;
    height: 100%;
  }
</style>
