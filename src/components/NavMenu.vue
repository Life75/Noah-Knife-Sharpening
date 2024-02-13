<template>
    <div id="NavMenu">
        <div class="flex md:align-middle pt-4  md:justify-end justify-center ">
            <div v-show="isMobile()" @click="showMenu = true">
                <div class="lineHelper"></div>
                <div class="lineHelper"></div>
                <div class="lineHelper"></div>
            </div>
            <p v-show="isMobile()" class="text-center md:pl-14 md:text-3xl text-2xl font-semibold m-auto">Noah's Knife Sharpening</p>
            
            <div v-show="!isMobile()" class="pt-1 ml-auto flex">
                <p>Made by Austyn Washington. Want a custom website like this?</p>
                <el-link href="https://awashington.notion.site/Hi-I-m-Austyn-fa6d777cd1a4409faf3fdd734b44cb03?pvs=4" type="primary" class="text pl-3">Contact me here</el-link>
            </div>    
        </div>
        <hr class="h-px my-4  border-0 bg-[#E5EAF3] opacity-25">
        
        <div class="flex justify-center align-middle py-4">
            <el-avatar class=" " :size="115" src="/assets/small_icon_businness_logo-e817294b.png"/>
        </div>
        <div v-show="!isMobile()" class="flex justify-center align-middle text-center   py-5   ">
            <p class="text-7xl m-auto font-semibold flex">Noah's Knife <p class="pl-3 " style="text-decoration: underline;">Sharpening</p></p>
        </div>
        <div v-show="!isMobile()" class="flex justify-center align-middle space-x-20 text-center text-2xl cursor-default " style="">
                <a href="https://noahsknifesharpening.as.me/schedule/6368d14f">
                    <p className=" relative group">
                        <div class="cursor-pointer hover-underline-animation">Make An Appointment</div>
                    <span className="absolute z-10 -bottom-1 left-0 w-0 h-0.5 bg-white transition-all group-hover:w-full"></span>
                    </p>
                </a>
                <a href="#testimonals">
                    <p className=" relative group">
                        <div class="cursor-pointer hover-underline-animation"> Testimonials</div>
                    <span className="absolute -bottom-1 left-0 w-0 h-0.5 bg-white transition-all group-hover:w-full"></span>
                    </p>
                </a>
                <a href="#instructions">
                    <p className=" relative group ">
                        <div class="cursor-pointer hover-underline-animation">Instructions</div>
                    <span className="absolute -bottom-1 left-0 w-0 h-0.5 bg-white transition-all group-hover:w-full"></span>
                    </p>
                </a>

                <a href="#contactUs">
                    <p className=" relative group">
                        <div class="cursor-pointer hover-underline-animation">Contact Us</div>
                    <span className="absolute -bottom-1 left-0 w-0 h-0.5 bg-white transition-all group-hover:w-full"></span>
                    </p>
                </a>
        </div>
        <el-drawer v-model="showMenu" :with-header="true" size="70%" direction="ltr" style="background-color: #3b3837 ">
            <a href="https://noahsknifesharpening.as.me/schedule/6368d14f">
                <p class="p-2 text-xl">Make an Appointment</p>
            </a>
            <a href="#testimonals" @click="()=> {showMenu = false}">
                <hr class="border-t-2 border-solid ">
                <p class="p-2 text-xl">Testimonals</p>
            </a>
            
            <a href="#instructions" @click="()=> {showMenu = false}">
                <hr class="border-t-2 border-solid ">
                <p class="p-2 text-xl">Instructions</p>
            </a>
            
            <a href="#contactUs" @click="()=> {showMenu = false}">
                <hr class="border-t-2 border-solid ">
                <p class="p-2 text-xl">Contact Us</p>
            </a>
        </el-drawer>
    </div>
</template>


<script setup lang="ts">
import { ref } from 'vue'
import { isMobile } from "../composables/PhoneCheckComposable"
/*
const state = reactive({
  circleUrl:
    ("../"),
})
*/
//const { circleUrl } = toRefs(state)

const showMenu = ref(false)
</script>

<style>
.lineHelper {
    width: 27px;
  height: 2px;
  background-color: white;
  margin: 6px 0;
}

.hover-underline-animation {
  display: inline-block;
  position: relative;
  color: whitesmoke;
}

.hover-underline-animation::after {
  content: '';
  position: absolute;
  width: 100%;
  transform: scaleX(0);
  height: 2px;
  bottom: 0;
  left: 0;
  background-color: whitesmoke;
  transform-origin: bottom right;
  transition: transform 0.25s ease-out;
}

.hover-underline-animation:hover::after {
  transform: scaleX(1);
  transform-origin: bottom left;
}

html{
     scroll-behavior: smooth;;
   }

</style>