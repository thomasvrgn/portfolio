<template>
  <div class="bg-gray-200 h-screen flex flex-row">
    <div class="flex flex-auto lg:w-4/6 lg:bg-gray-200">
      <div class="flex flex-auto justify-center items-center lg:justify-end">
        <div class="flex flex-initial justify-center items-center bg-white shadow-lg w-2/3 rounded-lg lg:rounded-none lg:rounded-l-lg lg:h-8/12">
          <div class="flex flex-col container lg:p-16">

            <div class="p-8 flex flex-row flex-wrap">
              <div class="flex flex-auto items-center lg:w-full">
                <div class="container lg:ml-2">
                  <h1 class="font-bold text-3xl text-gray-800">
                    Ness
                  </h1>
                  <p class="text-gray-600 font-light -mt-1">
                    Web developer
                  </p>
                </div>
              </div>
              <div class="flex flex-auto items-center">
                <div class="container flex flex-row flex-wrap justify-center lg:justify-start lg:mt-8">
                  <Button content="Button" color="red" />
                  <Button content="Button" color="purple" />
                  <Button content="Button" color="blue" />
                </div>
              </div>
            </div>

            <div class="container">
              <p class="font-normal px-8 pb-8 lg:px-10">
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Provident fuga sapiente blanditiis reiciendis maxime debitis iste tenetur architecto dolorum! Delectus eum soluta aut officia dolore consequuntur, velit inventore dolor! Quos.Quia incidunt quasi quisquam nobis in consequatur ipsam numquam corporis mollitia aperiam accusamus autem, deleniti illo sint quod, rem vero laboriosam repellat porro sequi molestiae optio? Obcaecati omnis alias asperiores.
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="flex-auto lg:w-2/6 bg-blue-500 hidden lg:flex items-center">
      <div class="container h-8/12">
        <img src="http://images.askmen.com/1080x540/2016/01/25-021526-facebook_profile_picture_affects_chances_of_getting_hired.jpg" class="h-full w-3/4 rounded-r-lg shadow-lg object-cover" alt="">
      </div>
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
