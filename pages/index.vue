<template>
  <Header />
</template>

<script lang="ts">
import Vue from 'vue'
import Header from '@/components/Header.vue'

export default Vue.extend({
  components: {
    Header
  }
})
</script>

<style lang="scss">
@import '@/node_modules/normalize.css/normalize.css';
html, body #__nuxt, #__layout, #__layout div {
  min-height: 100vh;
}
</style>