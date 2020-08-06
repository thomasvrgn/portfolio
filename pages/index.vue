<template>
  <Header>
    <Navbar />
    <Hero />
  </Header>
</template>

<script lang="ts">
import Vue from 'vue'
import Header from '~/components/Header.vue'
import Navbar from '~/components/Navbar.vue'
import Hero from '~/components/Hero.vue'

export default Vue.extend({
  components: {
    Header,
    Navbar
  }
})
</script>