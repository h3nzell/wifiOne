<style>
.title {
  font-weight: 300;
  font-size: 20px;
}
.support-section {
  line-height: 25px;
}
.description {
  color: #343E59;
  font-size: 20px;
  font-weight: 700;
}
.support-info {
  font-weight: 400;
  font-size: 20px
}
</style>
<template>
  <section  class="iq-bg-over pt-5 pb-5">
    <div class="container">
      <div class="w-100">
        <div class="col-md-12  mb-0 mb-lg-30 fadeInUp  wow d-flex justify-content-between flex-wrap">
          <div class="mt-3">
            <div class="mt-[35px] support-section">
              <p class="mb-0 text-primary title">Main Phone Number</p>
              <p class="mb-0 support-info">U.S.(800) 123-4678</p>
              <p class="mb-0 support-info">International +1(801)123-4567</p>
            </div>
            <div class="mt-3 support-section" >
              <p class="mb-0 text-primary title">Sales</p>
              <p class="mb-0 support-info">(800) 123-4678</p>
              <p class="mb-0 support-info">(800) 123 4569</p>
            </div>
          </div >
          <div class="mt-3">
            <div class="mt-[35px] support-section">
              <p class="mb-0 text-primary title">Technical Support</p>
              <p class="mb-0 support-info">(800) 123-4567</p>
              <p class="mb-0 support-info">(800) 123-4567</p>
            </div>
            <div class="mt-3 support-section" >
              <p class="mb-0 text-primary title">Mailing Address</p>
              <p class="mb-0 support-info">1 Keong Saik Road,</p>
              <p class="mb-0 support-info">Singapore 089109</p>
            </div>
          </div>
          <div class="mt-3">
            <h6 class="description">We Provide same-day equipment<br> replacement, and can reconfigure as your <br> needs change</h6>
            <button
              id="submit-4"
              click="/contact-us"
              name="submit"
              type="submit"
              value="Send"
              class="button  blue-btn mt-3 form-button"
            >
              Submit support ticket
            </button>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  name: 'Support',
}
</script>
 <style>
  .form-button {
    font-size: 14px;
  }
 </style>
