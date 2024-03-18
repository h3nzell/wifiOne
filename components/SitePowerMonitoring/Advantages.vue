<template>
  <section class="pt-0">
    <div class="container">
      <div class="row">
        <div class="col-lg-4 col-md-12  mx-auto" v-for="(list,index) in items" :key="index">
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
          title: 'Automated Notification for Site Power Loss',
          description: 'Immediate and automated alerts in case of site power loss, facilitating prompt response and risk mitigation.',
          src: require('../../assets/images/home/services/14.png')
        },
        {
          title: 'Risk Management for Electromagnetic Doors',
          description: 'Monitoring and risk management services for electromagnetic doors, ensuring secure operations and responsiveness in case of issues.',
          src: require('../../assets/images/home/services/10.png')
        },
      ]
    }
  }
}
</script>

<style>

</style>

