<script setup lang="ts">
//import Main from './components/Main.vue';
import NavMenu from "./components/NavMenu.vue";
import { isMobile } from "./composables/PhoneCheckComposable";
//function isMobile() {
//   if(/Android|webOS|iPhone|iPad|iPod|BlackBerry|IEMobile|Opera Mini/i.test(navigator.userAgent)) {
//     return true
//   } else {
//     return false
//   }
//  }

</script>

<template>
  <div v-show="!isMobile()" id="backdrop" class="absolute brightness-50">
  </div>
  
  <div
    id="page-container"
    class="flex-col"
    style="
      margin-right: 5%;
      margin-left: 5%;
      flex-direction: column;
      gap: 4em;
      height: 100vh;
      margin: 0 5%;
      font-family: Cormorant;
    "
  >

    <NavMenu></NavMenu>

  
    <div v-show="!isMobile()" class="flex justify-center align-middle text-center pt-52  ">
    <p class="text-7xl m-auto font-semibold">Noah's Knife Sharpening</p>
    </div>

  </div>

 
</template>

<style>
#backdrop {
  /* Background pattern from Toptal Subtle Patterns */
  background-image: url('assets/images/sword.jpg');
  height: 70%;
  width: 100%;
  z-index: -20;
  background-repeat: no-repeat;
  background-position: center; 
  
}
#page-container {
  position: relative;
  min-height: 100vh;
}

#content-wrap {
  padding-bottom: 2.5rem; /* Footer height */
}

#footer {
  position: absolute;
  bottom: 0;
  width: 40%;
  left: 80%;
  align-self: flex-end;
  height: 2.5rem; /* Footer height */
}

@font-face {
  font-family: Cormorant;
  src: url("assets/fonts/Cormorant-VariableFont_wght.ttf");
}
</style>
