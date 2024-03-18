<template>
  <section class="pt-0">
    <div class="container">
      <div class="row ">
        <div class="col-lg-4 col-md-12 mx-auto" v-for="(list,index) in items" :key="index">
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
          title: 'Multi-Zone Control',
          description: 'Centralized control and management of multiple zones, allowing for customized settings and operations in distinct areas.',
          src: require('../../assets/images/home/services/04.png')
        },
      ]
    }
  }
}
</script>

<style>

</style>

