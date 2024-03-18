<template>
  <section>
    <h1 class="text-center studies">CASE STUDIES</h1>
    <div class="container customer-studies-container">
      <img src="../../assets/images/customers/hotel-xoai.webp" alt="logo">
      <h2 class="text-center text-white studies-title">Hotel Xoai</h2>
      <p class="text-center text-white studies-text">
        Hotel Xoai, Can Tho, Vietnam
        <br>
        30 rooms over 6 floors, managed WiFi from wifiOne
        <br>
        <br>
        Hotel Xoai engaged wifiOne to setup and manage the hotel guest and operations network. After initial
        <br>
        setup, issues were quickly resolved with older cabling. The WiFi was carefully tuned to give reliable
        <br>
        coverage in all areas.
        <br>
        <br>
        This enabled the hotel to focus on business operations with no downtime.
      </p>
      <div class="author">
        <img src="../../assets/images/customers/avatar.webp" alt="avatar">
        <div class="text-white">
          <h4 class="text-white author-name">John Milligan</h4>
          <p class="author-text">CEO</p>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
export default {
name:'Studies'
}
</script>
<style>

 .studies {
   color: #3F81D1;
   font-size: 30px;
   font-style: normal;
   font-weight: 600;
   line-height: normal;
   margin-bottom: 50px;
 }
 .customer-studies-container {
   background-image: url("../../assets/images/customers/base-bg.webp");
   background-position: center;
   background-repeat: no-repeat;
   background-size: cover;
   padding: 100px;
   display: flex;
   flex-direction: column;
   align-items: center;
   justify-content: center;
   gap: 14px;
 }
 .studies-title {
   font-size: 35px;
   font-style: normal;
   font-weight: 600;
   line-height: normal;
 }
 .studies-text {
   text-align: center;
   font-size: 20px;
   font-style: normal;
   font-weight: 400;
 }
 .author {
   display: flex;
   gap: 20px;
   align-items: start;
 }
 .author-name {
   color: #FFF;
   font-size: 20px;
   font-style: normal;
   font-weight: 600;
   line-height: normal;
   margin-bottom: 4px;
 }
 .author-text {
   font-size: 17px;
   font-style: normal;
   font-weight: 600;
   line-height: normal;
 }
 @media (max-width: 600px) {
   .customer-studies-container {
     padding: 50px 10px;
   }
 }
</style>
