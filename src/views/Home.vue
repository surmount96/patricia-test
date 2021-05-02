<template>
  <div class="">
    <div class="flex lg:items-center flex-wrap lg:justify-start justify-center h-25 w-full">
      <div class="lg:flex lg:items-center lg:flex-wrap">
        <div class="lg:flex lg:items-baseline relative hidden lg:w-7/12 w-full lg:mb-0 md:mb-0 mb-6">
          <div class="flex items-baseline">
            <div class="pb-10 pr-6">
              <img src="@/assets/patricia-logo.svg" alt="patricia-logo">
            </div>
            <div class="flex flex-wrap items-baseline">
              <div class="w-8/12">
                <img src="@/assets/patricia.svg" alt="patricia"  class="h-50 object-cover ">
              </div>
              <div class="flex w-4/12">
                <img src="@/assets/VALID-THRU.svg" alt="valid-thru">
                <p class="ml-3 mr-5">
                  10/12
                </p>
              </div>
            </div>
          </div>
<!--          <div class="flex items-center w-3/12">-->
<!--            <div class="flex">-->
<!--              <img src="@/assets/VALID-THRU.svg" alt="valid-thru">-->
<!--              <p class="ml-3">-->
<!--                10/12-->
<!--              </p>-->
<!--              <p>-->
<!--                422-->
<!--              </p>-->
<!--            </div>-->
<!--          </div>-->
          <div class="absolute top-0 right-0 mr-12">
            <div class="flex justify-between flex-col h-50 pt-8">
              <img src="@/assets/Mask-open.svg" alt="patricia-logo" class="cursor-pointer">
              <p>
                422
              </p>
            </div>
          </div>
        </div>
        <div class="lg:w-5/12 w-full lg:mb-0 md:mb-0 mb-6 lg:pt-0 md:pt-0 pt-5">
          <div class="bg-dark rounded-custom col h-50 relative lg:ml-auto mx-auto">
            <div class="bg-image"></div>
            <div class="absolute flex flex-col justify-between top-0 w-full px-12-custom h-full">
              <div class="flex justify-between">
                <img src="@/assets/patricia-logo.svg" alt="patricia-logo">
                <img src="@/assets/Mask.svg" v-show="show" alt="patricia-logo" class="cursor-pointer" @click="show = false">
                <img src="@/assets/Mask-open.svg" v-show="!show" alt="patricia-logo" class="cursor-pointer" @click="show = true">
              </div>
              <div class="flex justify-between items-center w-full text-gray">
                <p class="h5">
                    <span v-show="show">
                      9784
                    </span>
                  <span class="h4" v-show="!show">
                      &#8226;
                      &#8226;
                      &#8226;
                      &#8226;
                    </span>
                </p>
                <p class=" h5">
                    <span v-show="show">
                      9784
                    </span>
                  <span class="h4"  v-show="!show">
                      &#8226;
                      &#8226;
                      &#8226;
                      &#8226;
                    </span>
                </p>
                <p class=" h5">
                    <span v-show="show">
                      9784
                    </span>
                  <span class="h4"  v-show="!show">
                      &#8226;
                      &#8226;
                      &#8226;
                      &#8226;
                    </span>
                </p>
                <p class=" h5">
                  9784
                </p>
              </div>
              <div class="flex justify-between items-center">
                <p class="card-text">
                  Cardholder name
                </p>
                <div class="flex items-center">
                  <div class="flex mx-4">
                    <img src="@/assets/VALID-THRU.svg" alt="valid-thru">
                    <p class="px-2">
                      10/12
                    </p>
                  </div>
                  <div class="flex items-center">
                    <p class="mr-2">
                      cvv
                    </p>
                    <p class="h5">
                      &#8226;
                      &#8226;
                      &#8226;
                    </p>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="lg:px-24">
      <div class="bg-dark rounded-custom col h-50 flex items-center px-12 lg:mb-0 md:mb-0 mb-6">
        <div class="flex justify-between items-center text-gray w-full">
          <p class="h5">
            9784
          </p>
          <p class="h5">
            9784
          </p>
          <p class="h5">
            9784
          </p>
          <p class="h5">
            9784
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  data(){
    return{
      show:false
    };
  },
  components: {
    HelloWorld
  }
}
</script>

<style>
.h-25{
  height: 70vh;
}

@media screen and (max-width: 600px) {
  .h-25{
    height: auto;
  }
}
</style>
