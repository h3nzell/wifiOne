<template>
  <section class="customers-office-and-business-top">
    <div class="container">
      <div class="customers-top-wrapper">
        <h1 class="text-white">Offices and Businesses</h1>
        <p class="text-white customers-top-text">Enhance productivity and communication within corporate <br> environments.</p>
        <div class="text-left">
          <a class="button blue-btn button-icon text-left" href="/contact-us"><span class="btn-effect"> Contact Us</span></a>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  name:'Hero'
}
</script>
<style>
.customers-office-and-business-top{
  background-image: url("../../assets/images/customers/office-and-business-hero.webp");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  background-color: #dedede;
}

.customers-top-text {
  font-size: 21px;
}

.customers-top-wrapper {
  display: flex;
  flex-direction: column;
  align-items: start;
  justify-content: start;
  gap: 31px;
  height: 100%;
}
</style>
