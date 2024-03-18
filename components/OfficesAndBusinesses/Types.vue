<template>
  <section class="">
    <div class="container">
      <div class="row">
        <div class="col-lg-4 col-md-6 mb-4" v-for="(list,index) in items" :key="index">
          <CardStyle1>
            <div slot="cardMedia" class="mb-2">
              <img :src="list.src" alt="fancy-list" class="mx-auto">
            </div>
            <div slot="cardTitle">
              <h5 class="mb-2">{{ list.title }}</h5>
            </div>
            <div slot="cardBody">
              <p class="">{{ list.description }}</p>
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
  name: 'Types',
  components: { CardStyle1 },
  data() {
    return{
      items : [
        {
          title: 'Smart Business Value',
          description: 'Aligns with your revenue stream, ensuring a cost-effective solution.',
          src: require('../../assets/images/home/services/08.png')
        },
        {
          title: 'Secure by Design',
          description: 'WPA3 wireless security, multi-level IP firewalling, and Zero Trust options for maximum wired security.',
          src: require('../../assets/images/home/services/09.png')
        },
        {
          title: 'Professional Network Design',
          description: 'Crafted with industry best practices, segmentation, and security for optimal performance.',
          src: require('../../assets/images/home/services/10.png')
        },
        {
          title: 'Captive Portal Option',
          description: 'Customized portal reflecting your brand, mindshare, or advertising upon network connection.',
          src: require('../../assets/images/home/services/01.png')
        },
        {
          title: 'Optimized Video Calling',
          description: 'Experience network fairness with Quality of Service. Prevent resource abuse and ensure smooth video calls during media traffic.',
          src: require('../../assets/images/home/services/11.png')
        },
        {
          title: 'Per-Tenant Network',
          description: 'Distinct network for each tenant in shared offices. Ensures optimal security, separation, and secure one-way device access in wifiONE\'s system.',
          src: require('../../assets/images/home/services/01.png')
        },
        {
          title: 'Managed VPN Option',
          description: 'Integration of a Virtual Private Network (VPN) with management services, ensuring secure and efficient communication across networks.',
          src: require('../../assets/images/home/services/06.png')
        },
        {
          title: '5G Backup Internet Option',
          description: 'Guarantees uninterrupted connectivity with a reliable backup option.',
          src: require('../../assets/images/home/services/02.png')
        }
      ]
    }
  }
}
</script>
