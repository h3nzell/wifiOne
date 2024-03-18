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
import Analytics from '~/components/ManagedMediaWall/Analytics'
import Footer from '~/components/ManagedMediaWall/Footer'
import Hero from '~/components/ManagedMediaWall/Hero.vue'
import { themes } from '../../assets/app/app'
import ContactUs from "~/components/ManagedMediaWall/ContactUs.vue";
import Advantages from "~/components/ManagedMediaWall/Advantages.vue";
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
      title: 'Media Wall and Signage | wifiOne',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'wifiOne\'s Managed Media Wall and Signage service is designed to enhance communication through dynamic and effective message delivery.'
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
