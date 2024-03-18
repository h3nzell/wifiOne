<template>
  <div class="main-content">
    <Hero/>
    <Analytics />
    <Advantages/>
    <ContactUs/>
    <Footer />
  </div>
</template>

<script>
import Analytics from '~/components/SitePowerMonitoring/Analytics'
import Footer from '~/components/SitePowerMonitoring/Footer'
import Hero from '~/components/SitePowerMonitoring/Hero.vue'
import { themes } from '../../assets/app/app'
import ContactUs from "~/components/SitePowerMonitoring/ContactUs.vue";
import Advantages from "~/components/SitePowerMonitoring/Advantages.vue";
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
      title: 'Site Power Monitoring | wifiOne',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'Automated notifications for site power loss, active electromagnetic doors, access control systems, seamless work of  online camera systems, easy fixing failures'
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
