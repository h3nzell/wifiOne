<template>
  <div class="image-loading">
    <div class="image-loading-center">
      <img :src="require('../../assets/images/loader.gif')" alt="loader">
    </div>
  </div>
</template>
<script>
export default {
  name: 'ImageLoader'
}
</script>
<style>
  .image-loading {
    position: absolute;
    height: 100%;
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: white;
    z-index: 1000;
    top:0;
  }
  .image-loading-center {
    background-color: inherit;
    height: 50px;
    width: 50px;
  }
</style>
