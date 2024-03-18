<template>
  <div class="main-content">
    <Hero/>
    <About/>
    <ContactUs/>
    <Types/>
    <Studies/>
    <ContactUs1/>
    <Footer/>
  </div>
</template>
<script>

import { themes } from '../../assets/app/app';
import Hero from '../../components/OfficesAndBusinesses/Hero.vue'
import About from '../../components/OfficesAndBusinesses/About.vue'
import Footer from "~/components/OfficesAndBusinesses/Footer.vue";
import ContactUs from "~/components/OfficesAndBusinesses/ContactUs.vue";
import Studies from "~/components/OfficesAndBusinesses/Studies.vue";
import ContactUs1 from "~/components/OfficesAndBusinesses/ContactUs1.vue";
import Types from "~/components/OfficesAndBusinesses/Types.vue";

export default {
  layout: 'Pages',
  components: {
    Types,
    Studies,
    ContactUs1,
    ContactUs,
    About,
    Footer,
    Hero,
  },
  head() {
    return {
      title: 'Offices and Businesses | wifiOne',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'Improve workplace productivity with wifiOne\'s services for offices and businesses. We offer high-performance WiFi solutions for your team.'
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
