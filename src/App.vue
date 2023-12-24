<script setup lang="ts">
//import Main from './components/Main.vue';
import NavMenu from "./components/NavMenu.vue";
import { isMobile } from "./composables/PhoneCheckComposable";
import Main from "./components/Main.vue"

</script>

<template>
  <div v-show="!isMobile()" id="backdrop" class="absolute brightness-50">
  </div>
  
  <div
    id="page-container"
    class="flex-col"
    style="
      @media (max-width: 800px) {}
      margin-right: 5%;
      margin-left: 5%;
      flex-direction: column;
      gap: 4em;
      margin: 0 5%;
      font-family: Cormorant;
    "
  >

    <NavMenu></NavMenu>

  



  </div>
  <Main style="
      margin-right: 5%;
      margin-left: 5%;
      flex-direction: column;
      gap: 4em;
   
      margin: 0 5%;
      font-family: Cormorant;
    "/>

</template>

<style>
#backdrop {
  /* Background pattern from Toptal Subtle Patterns */
  background-image: url('assets/images/knife_high_res.jpg');
  height: 60vh;
  width: 100%;
  z-index: -20;
  top: 0; 
  left: 0;
  background-repeat: no-repeat;
  background-position: center; 
  
}
#page-container {
  position: relative;      
  @media (max-width: 800px) {
    height: 20vh
  }
  height: 60vh;

}

#content-wrap {
  padding-bottom: 2.5rem; /* Footer height */
}


#wrapper {
  position: relative;
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
