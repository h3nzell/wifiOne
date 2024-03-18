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
  name: 'Services',
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
          title: 'Captive Portal Option',
          description: 'Customized portal reflecting your brand, mindshare, or advertising upon network connection.',
          src: require('../../assets/images/home/services/01.png')
        },
        {
          title: '5G SIM-Based Instant Deployment',
          description: 'Harnessing 5G tech for wire-free equipment placement. Optimize event support with strategic equipment locations in wifiONE\'s system.',
          src: require('../../assets/images/home/services/02.png')
        },
        {
          title: 'Pre-Event and During-Event Support',
          description: 'Comprehensive support services encompassing both pre-event preparations and on-site assistance during events. This offering ensures that clients receive assistance and guidance throughout the entire event lifecycle, from planning to execution.',
          src: require('../../assets/images/home/services/12.png')
        },
        {
          title: 'Managed VPN Event WiFi for Partners',
          description: 'Tailored WiFi solutions designed specifically for event partners, ensuring seamless connectivity and support during events. This service focuses on providing dedicated and reliable connectivity for partners involved in events and conferences.',
          src: require('../../assets/images/home/services/06.png')
        },
      ]
    }
  }
}
</script>
