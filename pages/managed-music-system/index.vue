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
import Analytics from '~/components/ManagedMusicSystem/Analytics'
import Footer from '~/components/ManagedMusicSystem/Footer'
import Hero from '~/components/ManagedMusicSystem/Hero.vue'
import { themes } from '../../assets/app/app'
import ContactUs from "~/components/ManagedMusicSystem/ContactUs.vue";
import Advantages from "~/components/ManagedMusicSystem/Advantages.vue";
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
      title: 'Managed Music Systems | wifiOne',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'Create the perfect ambiance with managed multi-zone music speakers and get full control, monitoring and management and user-friendly interface.'
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
