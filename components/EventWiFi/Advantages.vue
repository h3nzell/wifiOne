<template>
  <section class="pt-0">
    <div class="container">
      <div class="row">
        <div class="col-lg-6 col-md-12 mb-3" v-for="(list,index) in items" :key="index">
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
<script >
import CardStyle1 from "~/components/themes/Card/CardStyle1.vue";

export default {
  name: 'Advantages',
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
          title: '5G SIM-Based Instant Deployment',
          description: 'Harnessing 5G tech for wire-free equipment placement. Optimize event support with strategic equipment locations in wifiONE\'s system.',
          src: require('../../assets/images/home/services/02.png')
        },
        {
          title: 'Captive Portal Option',
          description: 'Customized portal reflecting your brand, mindshare, or advertising upon network connection.',
          src: require('../../assets/images/home/services/01.png')
        },
      ]
    }
  }
}
</script>

<style>
 .ppp {
  background-color: red;
 }
</style>

