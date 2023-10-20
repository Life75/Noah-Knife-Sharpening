<template>
    <div id="NavMenu">
        <div class="flex md:align-middle pt-4  md:justify-end justify-center ">
            <p v-show="isMobile()" class="text-center md:pl-14 md:text-3xl text-2xl font-semibold m-auto">Noah's Knife Sharpening</p>
            <div v-show="!isMobile()" class="pt-1">
                <svg class="cursor-pointer md:w-6 md:h-6 float-right " xmlns="http://www.w3.org/2000/svg" x="0px" y="0px" viewBox="0 0 48 48">
                    <path fill="#039be5" d="M24 5A19 19 0 1 0 24 43A19 19 0 1 0 24 5Z"></path><path fill="#fff" d="M26.572,29.036h4.917l0.772-4.995h-5.69v-2.73c0-2.075,0.678-3.915,2.619-3.915h3.119v-4.359c-0.548-0.074-1.707-0.236-3.897-0.236c-4.573,0-7.254,2.415-7.254,7.917v3.323h-4.701v4.995h4.701v13.729C22.089,42.905,23.032,43,24,43c0.875,0,1.729-0.08,2.572-0.194V29.036z"></path>
                </svg>
            </div>
            
        </div>
        <hr class="h-px my-4  border-0 bg-[#E5EAF3] opacity-25">
        
        <div class="flex justify-center align-middle py-4">
            <el-avatar class=" " :size="115" :src="circleUrl"/>
        </div>
        <div v-show="!isMobile()" class="flex justify-center align-middle space-x-20 text-center text-2xl cursor-default " style="">

                <p className=" relative group">
                    <div class="cursor-pointer">Make An Appointment</div>
                <span className="absolute -bottom-1 left-0 w-0 h-0.5 bg-white transition-all group-hover:w-full"></span>
                </p>

                <p className=" relative group">
                    <div class="cursor-pointer">Testimonials</div>
                <span className="absolute -bottom-1 left-0 w-0 h-0.5 bg-white transition-all group-hover:w-full"></span>
                </p>
                
                <p className=" relative group">
                    <div class="cursor-pointer">Call Now</div>
                <span className="absolute -bottom-1 left-0 w-0 h-0.5 bg-white transition-all group-hover:w-full"></span>
                </p>

                <p className=" relative group">
                    <div class="cursor-pointer">About Us</div>
                <span className="absolute -bottom-1 left-0 w-0 h-0.5 bg-white transition-all group-hover:w-full"></span>
                </p>
        </div>
    </div>
</template>


<script setup lang="ts">
import { reactive, toRefs } from 'vue'
import { isMobile } from "../composables/PhoneCheckComposable"

const state = reactive({
  circleUrl:
    '/src/assets/images/small_icon_businness_logo.png',
})

const { circleUrl } = toRefs(state)
</script>

<style>
</style>