<template>
  <section class="pt-[120px]">
    <div class="container">
      <h2 class="text-left mb-4">
        Let's talk about  your business
      </h2>
      <div class="row align-items-start ">
        <div class="col-sm-7">
          <div class="response-output" />
          <form action="/" method="post">
            <div class="contact-form">
              <div> <input type="text" name="your-name" class="form-control text " placeholder="Your Name"> </div>
              <div> <input type="text" name="your-email" class="form-control text " placeholder="Your Email"> </div>
              <div> <input type="text" name="your-subject" class="form-control text " placeholder="Website"> </div>
              <div> <textarea name="your-message" cols="40" rows="10" class="form-control textarea " placeholder="Your Message" /> </div>
              <div class="row">
                <div class="col-sm-12 col-md-4">
                  <button
                    id="submit-4"
                    click="/contact-us"
                    name="submit"
                    type="submit"
                    value="Send"
                    class="blue-btn button form-button"
                  >
                    Submit
                  </button>
                </div>
              </div>
            </div>
          </form>
        </div>
        <div class="mt-5  mx-0 col-sm-5 offset-lg-1 col-lg-5 offset-md-1 col-md-5">
          <div class="wrapper">
            <div class="contact-box d-flex justify-content-start align-items-start">
              <i aria-hidden="true" class="fa-regular fa-envelope"></i>
              <div class="service-detail">
                <h4 class="mb-2 contact-us-title">
                  Direct Email Contacts:
                </h4>
                <ul class="list-inline mb-0 contact-links">
                  <li><a href="mailto:support@iqnonicthemes.com"> General Inquiries: interact@wifione.co  </a></li>
                  <li><a href="mailto:support@iqnonicthemes.com"> Technical Support: wifi-support@wifione.co</a></li>
                  <li><a href="mailto:support@iqnonicthemes.com"> Sales and Partnerships: interact@wifione.co </a></li>
                </ul>
              </div>
            </div>
            <div class="contact-box d-flex justify-content-start  align-items-start">
              <i aria-hidden="true" class="ion ion-android-share-alt" />
              <div class="service-detail">
                <h4 class="mb-2 contact-us-title">
                  Social media
                </h4>
                <ul class="contact-links">
                  <li class="d-inline">
                    <a href="#"><i class="fa fa-facebook-f" /></a>
                  </li>
                  <li class="d-inline">
                    <a href="#"><i class="fa fa-twitter" /></a>
                  </li>
                  <li class="d-inline">
                    <a href="#"><i class="fa fa-instagram" /></a>
                  </li>
                </ul>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  name: 'ContactForm'
}
</script>
<style>
  .form-button {
    font-size: 14px;
  }
  .contact-us-title {
    color: #313E5B;
    font-size: 23px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
  }
  .contact-links {
    color: #515F81;
    font-size: 15px;
    font-style: normal;
    font-weight: 400;
  }
</style>
