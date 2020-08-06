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
@import url('https://fonts.googleapis.com/css2?family=Raleway:wght@100;200;300;400;500;600;700;800;900&display=swap');

* {
  box-sizing: border-box;
  margin: 0;
  font-family: 'Raleway', sans-serif;
  padding: 0;
}

html, body #__nuxt, #__layout, #__layout div {
  min-height: 100vh;
}
</style>