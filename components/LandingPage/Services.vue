<template>
  <section class="aboutus-two-service">
    <div class="container">
      <div class="row">
        <div class="col-lg-12">
          <div class="wow fadeInUp text-center mb-4">
            <span class="about-services-header">SERVICES</span>
          </div>
        </div>
      </div>
      <div class="row">
        <div class="col-lg-4 col-md-6 mb-5" v-for="(list,index) in items" :key="index">
          <CardStyle1>
            <div slot="cardMedia">
              <img :src="list.src" alt="fancy-list">
            </div>
            <div slot="cardTitle">
              <h4 class="mb-2">{{ list.title }}</h4>
            </div>
            <div slot="cardBody">
              <p>{{ list.description }}</p>
            </div>
            <div slot="cardInfo">
              <p class=" font-weight-bold mt-4">{{ list.info }}</p>
            </div>
            <div slot="cardLink">
              <div class="blog-button w-100 d-flex justify-content-end mt-3">
                  <a :href="list.link" class="button blue-btn button-icon text-left">Learn More</a>
              </div>
            </div>
          </CardStyle1>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
import CardStyle1 from '../themes/Card/CardStyle1'
export default {
  name: 'Services',
  components: { CardStyle1 },
  data() {
    return{
      items : [
        {
          title: 'Managed WiFI',
          info:'Suitable for business and offices',
          description: 'Enjoy the simplicity of network management with wifiOne. We provide comprehensive solutions to ensure your WiFi and network performance is always at its best. Benefit from uninterrupted connectivity, top-tier security, and reliability.',
          src: require('../../assets/images/home/services/01.png'),
          link: '/managed-wifi',
        },
        {
          title: 'Event WiFi',
          info:'Suitable for event organizers',
          description: 'Make your events memorable with wifiOne\'s Event WiFi service. Whether you\'re hosting a conference or a special gathering, we deliver reliable, high-performance connectivity. Keep your attendees connected and engaged.',
          src: require('../../assets/images/home/services/02.png'),
          link: '/event-wifi'
        },
        {
          title: 'Managed Cameras',
          info:'Ideal for service industry and offices',
          description: 'Ensure the safety and security of your premises with wifiOne\'s Managed Camera service. Our solution includes local storage for enhanced security, offering peace of mind and protection for your business.',
          src: require('../../assets/images/home/services/03.png'),
          link: '/managed-cameras'
        },
        {
          title: 'Managed Music Systems',
          info:'Ideal for service industry',
          description: 'Set the right mood with wifiOne\'s Managed Music System. With multi-zone control, you can customise your music experience in different areas. Create an ambiance that suits your space and your customers.',
          src: require('../../assets/images/home/services/04.png'),
          link: '/managed-music-system'
        },
        {
          title: 'Site Power Monitoring',
          info:'For companies with electromagnetic doors',
          description: 'Stay in control with wifiOne\'s Power Monitoring service. We keep an eye on your power systems, ensuring that your devices stay online and operational. No more unexpected downtimes or disruptions.',
          src: require('../../assets/images/home/services/05.png'),
          link: '/site-power-monitoring'
        },
        {
          title: 'Managed media wall',
          description: 'Transform your communication with wifiOne\'s Managed Media Wall and Signage service. Whether you prefer in-house updates or collaborate with our trusted digital content partners, we provide dynamic solutions to convey your message effectively and captivate your audience.',
          src: require('../../assets/images/home/services/06.png'),
          link: '/managed-media-wall',
        }
      ]
    }
  }
}
</script>
<style>
 .about-services-header {
   color:#3F81D1;
   font-size: 30px;
   font-style: normal;
   font-weight: 600;
 }
</style>
