<template>
  <section class="managed-music-top" id="managedMusicSystemTopSection">
    <ImageLoader v-if="loading" />
    <div class="container">
      <div class="row flex-nowrap">
        <div class="col-lg-10">
          <div class="managed-music-top-wrapper">
            <div class="wrapper-managed-music-title">
            <h1 class="text-white">Managed Music System</h1>
              <div class="col-lg-2 image ">
                <img src="/images/services/load.webp" alt="">
              </div>
            </div>
            <p class="text-white managed-music-top-text">Centralized control and management of multi-zone speaker systems for optimized audio
              <br> experiences in various areas.</p>
            <div class="text-left">
              <a class="button blue-btn button-icon text-left" href="/contact-us"><span class="btn-effect"> Contact Us</span></a>
            </div>
          </div>
        </div>
      </div>
      <div>
        <div class="loader-container ">
          <div class="rectangle-1"></div>
          <div class="rectangle-2"></div>
          <div class="rectangle-3"></div>
          <div class="rectangle-4"></div>
          <div class="rectangle-5"></div>
          <div class="rectangle-6"></div>
          <div class="rectangle-5"></div>
          <div class="rectangle-4"></div>
          <div class="rectangle-3"></div>
          <div class="rectangle-2"></div>
          <div class="rectangle-1"></div>
          <div class="rectangle-2"></div>
          <div class="rectangle-3"></div>
          <div class="rectangle-4"></div>
          <div class="rectangle-5"></div>
          <div class="rectangle-6"></div>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
import ImageLoader from "~/components/themes/ImageLoader.vue";

export default {
  name:'Hero',
  components: {ImageLoader},
  data() {
    return {
      loading: true,
    };
  },
  mounted() {
    const section = document.getElementById('managedMusicSystemTopSection');
    const backgroundImage = new Image();
    backgroundImage.src = "/images/services/manag-music-hero.webp";
    backgroundImage.onload = () => {
      section.classList.add('managed-music-system-top-image-loaded');
      this.loading = false;
    };
    backgroundImage.onerror = () => {
      section.classList.add('managed-music-system-top-image-loaded');
      this.loading = false;
    };
  },
}
</script>
<style>
.managed-music-top {
  position: relative;
  background-image: url("/images/services/manag-music-hero.webp");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  background-color: #dedede;
}
.managed-music-top-text {
  font-size: 21px;
}
.managed-music-system-top-image-loaded {
  background-image: url("/images/services/manag-music-hero.webp");
}
.managed-music-top-wrapper {
  display: flex;
  flex-direction: column;
  align-items: start;
  justify-content: start;
  gap: 31px;
  height: 100%;
}
.loader-container {
  gap: 15px;
  justify-content: center;
  display: flex;
  height: 40px;
  width: 100%;
  margin: 0px auto 0;
  mix-blend-mode: lighten;
}
.wrapper-managed-music-title {
  width: 100%;
  display: flex;
  justify-content: space-between;
}
.loader-container > div {
  position: relative;
  display: inline-block;
  background: #FFFFFF;
  border-radius: 3px;
  height: 100%;
  width: 10px;
  margin: 0;
  -webkit-animation: load 3s ease-in-out infinite;
  animation: load 3s ease-in-out infinite;
}

.loader-container .rectangle-2 {
  -webkit-animation-delay: 0.1s;
  animation-delay: 0.1s;
}

.loader-container .rectangle-3 {
  -webkit-animation-delay: 0.2s;
  animation-delay: 0.2s;
}

.loader-container .rectangle-4 {
  -webkit-animation-delay: 0.3s;
  animation-delay: 0.3s;
}

.loader-container .rectangle-5 {
  -webkit-animation-delay: 0.4s;
  animation-delay: 0.4s;
}

.loader-container .rectangle-6 {
  -webkit-animation-delay: 0.5s;
  animation-delay: 0.5s;
}

@-moz-keyframes load {
  0%,
  100% {
    -moz-transform: scaleY(1);
    background: #FFFFFF;;
  }
  16.67% {
    -moz-transform: scaleY(3);
    background: #FFFFFF;;
  }
  33.33% {
    -moz-transform: scaleY(1);
    background: #FFFFFF;;
  }
  50% {
    -moz-transform: scaleY(3);
    background: #FFFFFF;;
  }
  66.67% {
    -moz-transform: scaleY(1);
    background: #FFFFFF;;
  }
  83.34% {
    -moz-transform: scaleY(3);
    background: #FFFFFF;;
  }
}

@-webkit-keyframes load {
  0%,
  100% {
    -webkit-transform: scaleY(1);
    background:#FFFFFF;;
  }
  16.67% {
    -webkit-transform: scaleY(3);
    background: #FFFFFF;;
  }
  33.33% {
    -webkit-transform: scaleY(1);
    background: #FFFFFF;;
  }
  50% {
    -webkit-transform: scaleY(3);
    background: #FFFFFF;;
  }
  66.67% {
    -webkit-transform: scaleY(1);
    background: #FFFFFF;;
  }
  83.34% {
    -webkit-transform: scaleY(3);
    background: #FFFFFF;;
  }
}

@keyframes load {
  0%,
  100% {
    transform: scaleY(1);
    background: #FFFFFF;;
  }
  16.67% {
    transform: scaleY(3);
    background: #FFFFFF;;
  }
  33.33% {
    transform: scaleY(1);
    background: #FFFFFF;;
  }
  50% {
    transform: scaleY(3);
    background: #FFFFFF;;
  }
  66.67% {
    transform: scaleY(1);
    background: #FFFFFF;;
  }
  83.34% {
    transform: scaleY(3);
    background: #FFFFFF;
  }
}

.image {
  position: relative;
  max-width: 30%;
}

.image img {
  animation: rotate 3s infinite linear;
}

@keyframes rotate {
  0% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(360deg);
  }
}
</style>
