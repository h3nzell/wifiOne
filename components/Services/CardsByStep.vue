<template>
  <div class="container">
    <div class="cards-wrapper">
      <div class="work-card-wrapper">
        <img src="../../assets/images/services/works/arrow.png" alt="" class="arrow">
        <div class="work-card-img-wrapper">
          <img src="../../assets/images/services/works/work-1.png" alt="" class="work-card-img">
        </div>
        <h2 class="work-card-wrapper-title">Site Survey</h2>
        <p class="work-card-wrapper-text">Site survey will be conducted to comprehensively understand coverage and equipment requirements.</p>
      </div>
      <div class="work-card-wrapper">
        <img src="../../assets/images/services/works/arrow.png" alt="" class="arrow">
        <div class="work-card-img-wrapper">
          <img src="../../assets/images/services/works/work-2.png" alt="" class="work-card-img">
        </div>
        <h2 class="work-card-wrapper-title">Fiber Setup</h2>
        <p class="work-card-wrapper-text">The business will initiate the ordering process for an internet fiber plan from the Internet Service Provider (ISP) to establish the foundation for robust connectivity.</p>
      </div>
      <div class="work-card-wrapper">
        <div class="work-card-img-wrapper">
          <img src="../../assets/images/services/works/work-3.png" alt="" class="work-card-img">
        </div>
        <h2 class="work-card-wrapper-title">Installation</h2>
        <p class="work-card-wrapper-text">Cabling installation will be carried out to meet stringent 5GbE requirements, ensuring a high-quality and reliable network infrastructure.</p>
      </div>
    </div>
    <div class="cards-wrapper mt-5">
      <div class="work-card-wrapper">
        <img src="../../assets/images/services/works/arrow.png" alt="" class="arrow">
        <div class="work-card-img-wrapper">
          <img src="../../assets/images/services/works/work-4.png" alt="" class="work-card-img">
        </div>
        <h2 class="work-card-wrapper-title">Configuration</h2>
        <p class="work-card-wrapper-text">New equipment will be deployed, and multiple networks will be configured to optimize performance and meet specific business needs. Existing equipment will be seamlessly integrated.</p>
      </div>
      <div class="work-card-wrapper">
        <img src="../../assets/images/services/works/arrow.png" alt="" class="arrow">
        <div class="work-card-img-wrapper">
          <img src="../../assets/images/services/works/work-5.png" alt="" class="work-card-img">
        </div>
        <h2 class="work-card-wrapper-title">Validation</h2>
        <p class="work-card-wrapper-text">Rigorous validation processes will be implemented for both new and existing equipment and networks, ensuring functionality and performance. Staff will be involved in testing.</p>
      </div>
      <div class="work-card-wrapper">
        <div class="work-card-img-wrapper">
          <img src="../../assets/images/services/works/work-6.png" alt="" class="work-card-img">
        </div>
        <h2 class="work-card-wrapper-title">Monitoring</h2>
        <p class="work-card-wrapper-text">The commencement of infrastructure and key equipment monitoring, guaranteeing ongoing operational excellence through proactive monitoring measures.</p>
      </div>

    </div>
  </div>

</template>
<script>
export default {
  name:'CardsByStep'
}
</script>
<style>
 .cards-wrapper{
   width: 100%;
   display: flex;
   align-items: start;
   justify-content: start;
   gap:10px


 }
 .work-card-wrapper{
   position: relative;
   max-width: 33%;
   display: flex;
   flex-direction: column;
   align-items: center;
   justify-content: space-between;
   gap: 10px;
 }
 .work-card-wrapper-title {
   text-align: center;
   color: #343E59;
   font-size: 21px;
   font-style: normal;
   font-weight: 600;

 }
 .work-card-wrapper-text {
   text-align: center;
   color: #343E59;
   font-size: 16px;
   font-style: normal;
   font-weight: 400;
 }
 .arrow {
   position: absolute;
   left: 72%;
   display: block;
   width: 60%;
   z-index: 10;;
 }

 .work-card-img-wrapper {

 }
 .work-card-img{
   border: 5px solid #EFF1FE;
   border-radius: 50px;
   box-shadow:  #FAFBFE ;


 }
 @media (max-width: 600px) {
    .arrow {
      display: none;
    }
    .cards-wrapper {
      flex-direction: column;
    }
    .work-card-wrapper{
      max-width: 100%;
    }
 }
</style>
