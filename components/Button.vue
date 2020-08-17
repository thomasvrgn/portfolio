<template>
  <a href="" class="my-1 mx-2 py-2 px-6 rounded text-white font-semibold transition duration-300" :class="`bg-${color}-500 hover:bg-${color}-600 focus:bg-${color}-700`">
    {{ content }}
  </a>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  props: {
    color: String,
    content: String
  }
})
</script>