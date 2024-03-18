<template>
  <FooterMain class="footer-one iq-bg-dark iq-over-dark-90">
    <div slot="footerContent" class="footer-top">
      <div class="row">
        <div class="col-lg-4 col-md-6 col-sm-6">
          <FooterLogo
            :section-image="navLogo"
            section-text="wifiOne excels in delivering secure managed WiFi networks in Singapore, enssuring consistent connectivity. Explore how we transform your experience with the best-managed WiFi, keeping you at the forefront of WiFi technology."

          />
        </div>
        <div class="col-lg-2 col-md-6 col-sm-6 mt-4 mt-lg-0 mt-md-0">
          <FooterLinks :content="footerHome" title="Menu"/>
        </div>
        <div class="col-lg-6 col-md-6 col-sm-6 mt-lg-0 mt-4">
          <FooterAddress :address-content="footerText" address-title="Contact us" class="iq-contact" />
        </div>
      </div>
    </div>
  </FooterMain>
</template>
<script>
import FooterMain from '../themes/Partials/Footer/FooterMain'
import FooterLogo from '../themes/Partials/FooterComponents/FooterLogo'
import FooterAddress from '../themes/Partials/FooterComponents/FooterAddress'
import FooterLinks from '../themes/Partials/FooterComponents/FooterLinks'
import logoImg from '../../assets/images/logo_1.svg'

export default {
  name: 'Footer',
  components: {FooterLogo, FooterLinks, FooterAddress, FooterMain},
  data() {
    return {
      navLogo: logoImg,
      footerText: [
        {
          icon: true,
          iconClass: 'fas fa-phone-alt',
          text: '+0123 456 789'
        },
        {
          icon: true,
          iconClass: 'fas fa-envelope',
          text: 'interact@wifione.co'
        },
        {
          icon: true,
          iconClass: 'fas fa-location-dot',
          text: '1 Keong Saik Road, Singapore 089109'
        }
      ],
      footerHome: [
        {
          href: '/landing-page',
          title: 'Home'
        },
        {
          href: '/about',
          title: 'About'
        },
        {
          href: '/services',
          title: 'Services'
        },
        {
          href: '/customers',
          title: 'Customers'
        },
        {
          href: '/contact-us',
          title: 'Contact Us'
        }
      ]
    }
  }
}
</script>

<style scoped></style>
