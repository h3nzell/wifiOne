<template>
  <div class="main-content">
    <BreadCrum />
<!--    <Address />-->
    <ContactForm />
    <Map/>
    <SupportTitle/>
    <Support/>
    <Accordion/>
    <Footer />
  </div>
</template>

<script>
import BreadCrum from '../../components/ContactUs/BreadCrum'
import Address from '../../components/ContactUs/Address'
import ContactForm from '../../components/ContactUs/ContactForm'
import Footer from '../../components/ContactUs/Footer'
import { themes } from '../../assets/app/app'
import Accordion from "~/components/ContactUs/Accordion.vue";
import Support from "~/components/ContactUs/Support.vue";
import SupportTitle from "~/components/ContactUs/SupportTitle.vue";
import Map from "~/components/ContactUs/Map.vue";
export default {
  layout: 'ContactUs',
  head() {
    return {
      title: 'Contact us | wifiOne',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'Reach out through our contact us page to explore collaboration, get answers to your queries, or share feedback. We\'re here to assist you on your journey.'
        }
      ],
      link: [
        {rel: "preload", as: "image", href: '/images/home/bg2.svg'}
      ]
    }
  },
  components: {
    Map,
    SupportTitle,
    Support,
    Accordion,
    BreadCrum,
    Address,
    ContactForm,
    Footer
  },
  mounted () {
    setTimeout(function () {
      themes.index()
    }, 0)
  }
}
</script>
