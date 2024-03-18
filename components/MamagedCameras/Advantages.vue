<template>
  <section class="pt-0">
    <div class="container">
      <div class="row">
        <div class="col-lg-4 col-md-12 " v-for="(list,index) in items" :key="index">
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
          title: 'Dedicated Mobile App',
          description: 'Provision of a specialized mobile application for convenient and efficient management of services and connectivity on the go.',
          src: require('../../assets/images/home/services/01.png')
        },
        {
          title: 'Off-Site Viewing and History',
          description: 'Capability for remote viewing and access to historical data, allowing for comprehensive monitoring and analysis beyond on-site presence.',
          src: require('../../assets/images/home/services/09.png')
        },
      ]
    }
  }
}
</script>

<style>

</style>

