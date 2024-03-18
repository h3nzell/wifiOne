<template>
  <section class="pb-0">
    <div class="container">
      <div class="row">
        <div class="col-sm-12 wow fadeInUp">
          <div class="title-box wow fadeInUp text-center">
            <span class="clients-header">TRUSTED BY</span>
          </div>
        </div>
        <div class="col-md-12">
          <div
            class="owl-carousel owl-loaded owl-drag"
            data-dots="false"
            data-nav="false"
            data-items="6"
            data-items-laptop="4"
            data-items-tab="3"
            data-items-mobile="2"
            data-items-mobile-sm="1"
            data-dots-mobile="true"
            data-autoplay="true"
            data-loop="true"
            data-margin="30"
          >
            <div v-for="(item,index) in list" :key="index" class="item">
              <div class="clients-box">
                <img class="img-fluid client-img" :src="item.image" alt="image0">
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  name: 'Client',
  data () {
    return {
      list: [
        {
          image: require('../../assets/images/home/clients/1.png')
        },
        {
          image: require('../../assets/images/home/clients/2.png')
        },
        {
          image: require('../../assets/images/home/clients/3.png')
        },
        {
          image: require('../../assets/images/home/clients/4.png')
        },
        {
          image: require('../../assets/images/home/clients/5.png')
        },
        {
          image: require('../../assets/images/home/clients/6.png')
        },
        {
          image: require('../../assets/images/home/clients/7.png')
        },
        {
          image: require('../../assets/images/home/clients/8.png')
        },
        {
          image: require('../../assets/images/home/clients/9.png')
        },
        {
          image: require('../../assets/images/home/clients/10.png')
        },
        {
          image: require('../../assets/images/home/clients/11.png')
        },
      ]
    }
  }
}
</script>
<style>
 .clients-header {
   color: #3F81D1;
   font-size: 30px;
   font-style: normal;
   font-weight: 600;
   line-height: normal;
 }
</style>
