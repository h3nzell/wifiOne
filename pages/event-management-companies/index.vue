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
import Hero from '../../components/EventManagmentCompanies/Hero.vue'
import About from '../../components/EventManagmentCompanies/About.vue'
import Footer from "~/components/EventManagmentCompanies/Footer.vue";
import ContactUs from "~/components/EventManagmentCompanies/ContactUs.vue";
import Studies from "~/components/EventManagmentCompanies/Studies.vue";
import ContactUs1 from "~/components/EventManagmentCompanies/ContactUs1.vue";
import Types from "~/components/EventManagmentCompanies/Types.vue";

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
