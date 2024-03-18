<template>
  <section class="pt-0">
    <div class="container">
      <div class="row">
        <div class="col-md-12 wow fadeInUp title-box text-center">
          <span class="awards-title">Awards</span>
          <h2>Awards &amp; Accreditations</h2>
        </div>
      </div>
      <div class="row wow fadeInUp offset-lg-2 mx-auto">
        <div v-for="(option,index) in images2" :key="index" class="col-lg-4 col-md-4">
          <div class="xamin-award wow fadeInUp text-center">
            <div class="award-img"> <img :src="option.src" alt="fancybox"> </div>
            <h5 class="mt-3">{{ option.title }}</h5>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  name: 'Awards',
  data () {
    return {
      images2: [
        {
          title: 'Microsoft Partner of the Year Award',
          src: require('../../assets/images/awards/1.png')
        },
        {
          title: 'Global Sourcing Awards 2018 Finalist',
          src: require('../../assets/images/awards/2.png')
        },
        {
          title: 'Gold Winner of 2013 Horizon Awards',
          src: require('../../assets/images/awards/3.png')
        }
      ]
    }
  }
}
</script>
<style>
  .awards-title {
    color: #3F81D1;
    text-align: right;
    font-size: 30px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
    text-transform: uppercase;
  }
</style>
