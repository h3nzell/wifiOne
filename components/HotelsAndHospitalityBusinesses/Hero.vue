<template>
  <section class="hotels-and-hospitality-businesses-top">
    <div class="container">
      <div class="customers-top-wrapper">
        <h1 class="text-white">Hotels and Hospitality Businesses</h1>
        <p class="text-white customers-top-text">Elevate your guest experience with seamless and secure <br> connectivity.</p>
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
.hotels-and-hospitality-businesses-top{
  background-image: url("../../assets/images/customers/hotels-and-hospitality-businesses-hero.webp");
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
