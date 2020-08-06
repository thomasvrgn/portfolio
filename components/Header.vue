<template>
  <div class="container">
    <Navbar />
    <Hero />
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