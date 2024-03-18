<template>
  <div class="main-content">
<!--    <BreadCrum />-->
    <Hero/>
    <Analytics />
    <Advantages/>
    <ContactUs/>
    <Footer />
  </div>
</template>

<script>
import Analytics from '~/components/EventWiFi/Analytics'
import Footer from '~/components/EventWiFi/Footer'
import Hero from '~/components/EventWiFi/Hero.vue'
import { themes } from '../../assets/app/app'
import ContactUs from "~/components/EventWiFi/ContactUs.vue";
import Advantages from "~/components/EventWiFi/Advantages.vue";
export default {
  layout: 'Services',
  components: {
    Advantages,
    ContactUs,
    Analytics,
    Hero,
    Footer
  },
  head() {
    return {
      title: 'Event WiFi | wifiOne',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'wifiOne brings event WiFi solutions to events of all sizes. We specialize in providing secure, fast, and reliable connectivity-ideal or indoor and outdoor events.'
        }
      ],
    }
  },
  mounted () {
    setTimeout(function () {
      themes.index()
    }, 1000)
  }
}
</script>
