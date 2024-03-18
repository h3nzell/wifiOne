<template>
  <section class="event-management-companies-top">
    <div class="container">
      <div class="customers-top-wrapper">
        <h1 class="text-white">Event Management Companies</h1>
        <p class="text-white customers-top-text">Providing reliable WiFi solutions during events and conferences.</p>
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
.event-management-companies-top{
  background-image: url("../../assets/images/customers/event-management-companies-hero.webp");
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
