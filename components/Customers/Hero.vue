<template>
  <section class="customers-top" id="customersTopSection">
    <ImageLoader v-if="loading" />
    <div  class="container">
      <div class="customers-top-wrapper">
        <h1 class="text-white">Our Clients</h1>
        <p class="text-white customers-top-text">Crafting Connectivity for Diverse Businesses</p>
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
  components: { ImageLoader },
  data() {
    return {
      loading: true,
    };
  },
  mounted() {
    const section = document.getElementById('customersTopSection');
    const backgroundImage = new Image();
    backgroundImage.src = "/images/customers/customers-hero.webp";
    backgroundImage.onload = () => {
      section.classList.add('customers-top-image-loaded');
      this.loading = false;

    };
    backgroundImage.onerror = () => {
      section.classList.add('customers-top-image-loaded');
      this.loading = false;
    };
  },
}
</script>
<style>
.customers-top {
  background-image:  url("/images/customers/customers-hero.webp");
  position: relative;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  background-color: #dedede;
}
.customers-top-text {
  font-size: 21px;
}
.customers-top-image-loaded {
  background-image:  url("/images/customers/customers-hero.webp");
}
.customers-top-wrapper {
  display: flex;
  flex-direction: column;
  align-items: start;
  justify-content: start;
  gap: 31px;
  height: 100%;
}
</style>
