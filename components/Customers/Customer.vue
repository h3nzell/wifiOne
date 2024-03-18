<template>
  <section class="customers">

    <div class="office py-5">
      <div class="container">
        <div class="row ">
          <div class="col-lg-4 col-sm-12 d-flex justify-content-center">
            <img src="../../assets/images/customers/office-1.webp" alt="">
          </div>
          <div class="col-lg-8 col-sm-12 customer-info">
            <h1 class="text-left customers-title">CUSTOMERS</h1>
            <h2 class="customer-title">Office-Based Businesses</h2>
            <p>Transform your office into a hub of productivity and seamless communication with wifiOne. Our tailored solutions ensure reliable and high-performance WiFi, empowering your team to collaborate efficiently and drive success.</p>
            <div class="text-left">
              <a class="button blue-btn button-icon text-left" href="/offices-and-businesses"><span class="btn-effect">Learn More</span></a>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="companies py-5">
      <div class="container">
        <div class="row ">
          <div class="col-lg-8 col-sm-12 customer-info">
            <h2 class="customer-title">Event Management Companies</h2>
            <p>Deliver exceptional experiences during events, conferences, and gatherings with wifiOne's reliable WiFi solutions. From seamless attendee connectivity to robust event management, we ensure your events run smoothly, leaving a lasting impression on participants.</p>
            <div class="text-left">
              <a class="button blue-btn button-icon text-left" href="/event-management-companies"><span class="btn-effect">Learn More</span></a>
            </div>
          </div>
          <div class="col-lg-4 col-sm-12 d-flex justify-content-center">
            <img src="../../assets/images/customers/company-1.webp" alt="">
          </div>
        </div>
      </div>
    </div>
    <div class="hotels py-5">
      <div class="container">
        <div class="row ">
          <div class="col-lg-4 col-sm-12 d-flex justify-content-center">
            <img src="../../assets/images/customers/htel-1.webp" alt="">
          </div>
          <div class="col-lg-8 col-sm-12 customer-info">
            <h2 class="customer-title">Hotels and Hospitality Businesses</h2>
            <p>From hotels to restaurants and cafes, elevate guest satisfaction in hospitality establishments with wifiOne. Our solutions provide guests with uninterrupted and secure connectivity, enhancing their overall experience and ensuring your business stands out in the competitive hospitality landscape.</p>
            <div class="text-left">
              <a class="button blue-btn button-icon text-left" href="/hotels-and-hospitality-businesses"><span class="btn-effect">Learn More</span></a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  name:'Customer'
}
</script>
<style>
 .customers-title {
   color: #3F81D1;
   font-size: 30px;
   font-style: normal;
   font-weight: 600;
   line-height: normal;
 }
 .customer-info {
   display: flex;
   flex-direction: column;
   gap: 30px;
 }
 .customer-title {
   color: #343E59;
   font-size: 40px;
   font-style: normal;
   font-weight: 600;
   line-height: normal;
 }
 .companies {
   background-color: #EFF1FD;
 }
</style>
