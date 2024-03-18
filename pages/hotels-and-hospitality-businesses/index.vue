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
import Hero from '../../components/HotelsAndHospitalityBusinesses/Hero.vue'
import About from '../../components/HotelsAndHospitalityBusinesses/About.vue'
import Footer from "~/components/HotelsAndHospitalityBusinesses/Footer.vue";
import ContactUs from "~/components/HotelsAndHospitalityBusinesses/ContactUs.vue";
import Studies from "~/components/HotelsAndHospitalityBusinesses/Studies.vue";
import ContactUs1 from "~/components/HotelsAndHospitalityBusinesses/ContactUs1.vue";
import Types from "~/components/HotelsAndHospitalityBusinesses/Types.vue";

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
      title: 'Hospitality | wifiOne',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'Transform guest experiences in the hospitality industry with reliable WiFi solutions. Get seamless connectivity, guest satisfaction, and higher service standards. '
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
