<template>
<section class="ideas mb-5">
<div class="container">
  <div class="row align-items-center ">
    <div class="col-sm-4 d-none d-lg-block">
      <img src="../../assets/images/about-us/man.webp" alt="man" class="ideas-man">
    </div>
    <div class="mt-5 col-sm-12 col-lg-8">
      <h1 class="ideas-title text-center mb-0">We’re in The Business of Hosting Great Ideas.</h1>
      <p class="ideas-text text-center">"To empower businesses with performant, secure, and affordable <br> managed WiFi and network solutions, enabling them to thrive in the
        <br>
        connected world"
      </p>
      <div class="d-flex align-items-center justify-content-center">
        <img src="../../assets/images/about-us/man-mini.webp" alt="Man-mini" class="man-mini d-block d-lg-none">
        <p class="ideas-author text-center mt-0">Daniel Blueman</p>
      </div>

    </div>
  </div>
</div>
</section>
</template>
<script>
export default {
  name: 'Ideas'
}
</script>
<style>
  .ideas-title {
    color: #343E59;
    font-size: 32px;
    font-weight: 400;
  }
  .ideas {
    background-color: #F0F2FD;
    padding: 48px 0;
    margin-top:50px;
    background-image: linear-gradient(to right, #F0F2FD, #FFFFFF);
  }
  .ideas-text {
    color: #343E59;
    font-size: 19px;
    font-weight: 400;
  }
  .ideas-man {
    position: absolute;
    bottom: -180px;
  }
  .ideas-author {
    color: #3F81D1;
    font-size: 20px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
    margin-bottom: 0;
  }
  .man-mini {
    border-radius: 50px;
    margin-right: 10px;
  }
</style>
