<template>
  <div class="nessmc:app">
    <Navbar />
    <Hero />
    <div class="nessmc:container">
      <div class="nessmc:item nessmc:blank">
        <span></span>
      </div>
      <div class="nessmc:item nessmc:coloured">
        <span></span>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import Navbar from '@/components/Navbar.vue'
import Hero from '@/components/Hero.vue'

export default Vue.extend({
  components: {
    Navbar,
    Hero
  }
})
</script>

<style lang="scss" scoped>
.nessmc\:container {
  display: flex;
  flex-flow: row wrap;
  width: 100%;
  .nessmc\:item {
    display: flex;
    flex: 1 0;
    &.nessmc\:blank {
      flex-basis: calc(100% - 650px);
      background-color: rgb(240, 240, 240);
      @media (max-width: 1440px) {
        flex-basis: 50%;
      }
    }
    &.nessmc\:coloured {
      flex-basis: 650px;
      background-image: linear-gradient(to bottom, #a71cd8, #9123c6, #7c25b3, #6825a0, #56248c);
      @media (max-width: 1440px) {
        flex-basis: 50%;
      }
      @media (max-width: 1280px) {
        display: none;
      }
    }
  }
}
</style>