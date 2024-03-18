<template>
  <section>
    <h1 class="text-center studies">CASE STUDIES</h1>
    <div class="container customer-studies-container">
      <img src="../../assets/images/customers/fossasia.webp" alt="logo">
      <h2 class="text-center text-white studies-title">Fossasia</h2>
      <p class="text-center text-white studies-text">
        wifiOne has been supporting the FOSSASIA OpenTech conference in Singapore during its annual summit over the last 7 years. The conference spans multiple days, attracting over 1000 attendees per day.
        <br>
        <br>
        The largest deployment was 18 access points with over 550 users spanning 13 rooms; this enabled attendees real-time communications, interactive workshops and seamless connectivity throughout over all their devices.
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
