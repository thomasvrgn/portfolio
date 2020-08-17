<template>
  <div class="bg-gray-200 h-screen flex flex-row">
    <div class="flex flex-auto lg:w-3/4 lg:bg-red-200">
      <div class="flex flex-auto justify-center items-center">
        <div class="flex flex-initial justify-center items-center bg-white shadow-lg w-2/3 rounded-lg">
          <div class="container p-8 flex flex-row">
            <div class="flex flex-auto items-center">
              <div class="container">
                <h1 class="font-bold text-3xl text-gray-800">
                  Ness
                </h1>
                <p class="italic text-gray-600">
                  Web developer
                </p>
              </div>
            </div>
            <div class="flex flex-auto w-3/4 items-center">
              <div class="container flex flex-row flex-wrap justify-center">
                <Button content="Button" color="red" />
                <Button content="Button" color="purple" />
                <Button content="Button" color="blue" />
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="flex flex-auto lg:w-1/4 bg-blue-400 hidden">

    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import Button from './Button.vue'

export default Vue.extend({
  components: {
    Button
  }
})
</script>
