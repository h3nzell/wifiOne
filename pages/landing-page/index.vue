<template>
  <div>
    <div class="main-content">
      <Home />
      <Business/>
      <ChooseUs />
      <Counter />
      <Services />
      <ContactUs />
      <Testimonial />
      <Client />
      <Form />
      <ContactUs1/>
    </div>
    <Footer />
  </div>
</template>

<script>
import Counter from '../../components/LandingPage/Counter.vue';
import Home from '../../components/LandingPage/Home.vue';
import Testimonial from '../../components/LandingPage/Testimonial';
import ContactUs from '../../components/LandingPage/ContactUs.vue';
import ContactUs1 from '../../components/LandingPage/ContactUs1.vue';
import Services from '../../components/LandingPage/Services.vue';
import Footer from '../../components/LandingPage/Footer';
import { themes } from '../../assets/app/app';
import Business from "~/components/LandingPage/Business.vue";
import ChooseUs from "~/components/LandingPage/ChooseUs.vue";
import Client from "~/components/LandingPage/Client.vue";
import Form from "~/components/LandingPage/Form.vue";
export default {
  layout: 'LandingPage1',
  components: {
    Client,
    ChooseUs,
    Business,
    Home,
    Form,
    ContactUs,
    Counter,
    Services,
    Testimonial,
    ContactUs1,
    Footer
  },
  head() {
    return {
      title: 'Managed WiFi and Network Solutions',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'Reliable, high-performance networking tailored to your business needs. Experience seamless connectivity with our managed WiFi and network solutions'
        }
      ],
      link: [
        {rel: "preload", as: "image", href: '/images/home/bg2.svg'},
        {rel: "preload", fetchpriority: 'high', type: 'image/webp', as: "image", href: '/images/services/site-pwer-monitoring-hero.webp'},
        {rel: "preload", fetchpriority: 'high', type: 'image/webp', as: "image", href: '/images/services/hero.webp'},
        {rel: "preload", fetchpriority: 'high', type: 'image/webp', as: "image", href: '/images/services/wifi.webp'},
        {rel: "preload", fetchpriority: 'high', type: 'image/webp', as: "image", href: '/images/services/event-wifi-hero.webp'},
        {rel: "preload", fetchpriority: 'high', type: 'image/webp', as: "image", href: '/images/services/manag-cam-hero.webp'},
        {rel: "preload", fetchpriority: 'high', type: 'image/webp', as: "image", href: '/images/services/manag-music-hero.webp'},
        {rel: "preload", fetchpriority: 'high', type: 'image/webp', as: "image", href: '/images/services/managed-media-wall-hero.webp'},
        {rel: "preload", fetchpriority: 'high', type: 'video/webm', as: "video", href: '/videos/manag-wifi.webm'},
      ]
    }
  },
  mounted () {
    document.cookie = 'layout=LandingPage1'
    setTimeout(function () {
      themes.index()
      themes.initRevSlider19()
    }, 1000)
  }
}
</script>
