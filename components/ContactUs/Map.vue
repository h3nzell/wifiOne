<template>
  <section class="pt-0">
    <div class="container">
      <div class="row align-items-center">
        <div class="col-lg-12 col-md-12 w-fill">
          <div class = "address">
            <h2 class="address-text">For in-person visits or postal correspondence, you can find us at:</h2>
          </div>
          <div class = "address">
            <img src="../../assets/images/mark.png" alt="mark">
            <h2 class="address-title">1 Keong Saik Road, Singapore 089109</h2>
          </div>
          <div>
            <iframe
              height="590"
              allowfullscreen
              src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3988.607975594568!2d103.84276851475853!3d1.2811929990298014!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x31da18dca50d9b27%3A0x70d7a1e7ba020a3c!2s1%20Keong%20Saik%20Rd%2C%20Singapore%20089109!5e0!3m2!1sen!2ssg!4v1640137992449!5m2!1sen!2ssg"
            ></iframe>
          </div>

        </div>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  name:'Map'
}
</script>
<style>
  .address{
    display: flex;
    align-items: center;
    gap:20px;
    margin-bottom: 20px;
  }
  .address-title {
    font-size: 27px;
    font-weight: 700;
    color: #343E59;
  }
  iframe {
    border: none;
  }
  .address-text {
    color: #343E59;
    font-size: 27px;
    font-style: normal;
    font-weight: 600;
  }

</style>
