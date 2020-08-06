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
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@100;300;400;500;700;900&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Roboto+Slab:wght@100;300;500;700;900&display=swap');

* {
  box-sizing: border-box;
  margin: 0;
  font-family: 'Roboto', sans-serif;
  padding: 0;
}

html, body #__nuxt, #__layout, #__layout div {
  min-height: 100vh;
}
</style>