<template>
  <footer id="contact" :class="footerClass">
    <div class="container">
      <slot name="footerContent"></slot>
      <div class="copyright-footer">
        <div class="pt-3 pb-3">
          <div class="row flex-row-reverse justify-content-between">
            <div class="col-lg-12 col-md-12 text-lg-center text-md-center text-center"> <span class="copyright">Copyright 2024 <a href="/landing-page">WifiOne</a> All Rights Reserved.</span> </div>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>
<script>
export default {
  name: 'FooterMain',
  props: ['footerClass']
}
</script>
