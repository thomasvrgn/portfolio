<template>
  <div class="nessmc:hero">
    <div class="nessmc:hero-text">

    </div>
    <div class="nessmc:hero-banner">
      
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  
})
</script>

<style lang="scss">
.nessmc\:hero {
  position: absolute;
  top: 50%;
  left: calc(100% - 792px);
  transform: translate(-50%, -50%);
  height: 50%;
  min-height: unset !important;
  width: 950px;
  border-radius: 25px;
  box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
  display: flex;
  @media (max-width: 1440px) {
    width: 75%;
    height: 75%;
    left: 50%;
  }
  @media (max-width: 1280px) {
    flex-flow: row wrap;
  }
  .nessmc\:hero-text {
    min-height: unset !important;
    display: flex;
    flex: 1 0 65%;
    background: white;
    border-radius: 25px 0 0 25px;
    @media (max-width: 1440px) {
      flex: 1 0 50%;
    }
    @media (max-width: 1280px) {
      flex: 1 0 100%;
    }
  }
  .nessmc\:hero-banner {
    min-height: unset !important;
    display: flex;
    flex: 1 0 35%;
    background-image: url('../assets/logo.jpg');
    background-position: center center;
    background-size: cover;
    filter: grayscale(100%);
    border-radius: 0 25px 25px 0;
    @media (max-width: 1440px) {
      flex: 1 0 50%;
    }
    @media (max-width: 1280px) {
      flex: 1 0 100%;
    }
  }
}
</style>