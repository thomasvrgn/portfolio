<template>
  <div class="nessmc:container">
    <div class="nessmc:item nessmc:blank">
      <span></span>
    </div>
    <div class="nessmc:item nessmc:coloured">
      <span></span>
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
      flex-basis: 65%;
    }
    &.nessmc\:coloured {
      flex-basis: 35%;
      background-image: linear-gradient(to bottom, #a71cd8, #9123c6, #7c25b3, #6825a0, #56248c);
    }
  }
}
</style>