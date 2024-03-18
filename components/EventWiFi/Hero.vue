<template>
  <section class="event-wifi-top" id="EventWiFiTopSection">
    <ImageLoader v-if="loading" />
    <div class="container">
      <div class="event-wifi-top-wrapper">
        <h1 class="text-white">Event WiFi</h1>
        <p class="text-white event-wifi-top-text">Tailored WiFi solutions for events and conferences, providing reliable, high-performance connectivity with optional on-site management.</p>
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
    const section = document.getElementById('EventWiFiTopSection');
    const backgroundImage = new Image();
    backgroundImage.src = "/images/services/event-wifi-hero.webp";
    backgroundImage.onload = () => {
      section.classList.add('event-wifi-top-image-loaded');
      this.loading = false;
    };
    backgroundImage.onerror = () => {
      section.classList.add('event-wifi-top-image-loaded');
      this.loading = false;
    };
  },
}
</script>
<style>
.event-wifi-top {
  position: relative;
  background-image: url("/images/services/event-wifi-hero.webp");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  background-color: #dedede;
  height: 490px;
}
.event-wifi-top-text {
  font-size: 21px;
}
.event-wifi-top-image-loaded {
  background-image: url("/images/services/event-wifi-hero.webp");
}
.event-wifi-top-wrapper {
  display: flex;
  flex-direction: column;
  align-items: start;
  justify-content: start;
  gap: 31px;
  height: 100%;
}
</style>
