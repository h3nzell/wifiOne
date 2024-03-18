<template>
  <section class="aboutus-two-service">
    <div class="container">
      <div class="row mb-3">
        <div class="col-lg-12">
          <div class="title-box wow fadeInUp text-center">
            <span class="work-header">HOW IT WORKS</span>
            <h1 class="">How Does WifiOne Work</h1>
          </div>
        </div>
      </div>
    </div>
    <CardsByStep/>
  </section>
</template>
<script>
import CardStyle1 from '../themes/Card/CardStyle1'
import CardsByStep from "~/components/Services/CardsByStep.vue";
export default {
  name: 'Services',
  components: {CardsByStep, CardStyle1 },
  data() {
    return{
    }
  }
}
</script>
<style>
  .work-header {
    color: #3F81D1;
    font-size: 30px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
  }
</style>
