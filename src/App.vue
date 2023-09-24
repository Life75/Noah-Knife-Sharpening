<script setup lang="ts">
import Main from './components/Main.vue';
import NavMenu from './components/NavMenu.vue';
</script>

<template>
  <div id="page-container" class="flex-col" style="margin-right:5%; margin-left: 5%;  flex-direction:column; gap: 4em; height: 100vh; margin: 0 5%; font-family: Cormorant;">
    <NavMenu></NavMenu>

    <Main class="text-center"></Main>
  </div>
</template>

<style >
#page-container {
  position: relative;
  min-height: 100vh;
}

#content-wrap {
  padding-bottom: 2.5rem;    /* Footer height */
}

#footer {
  position: absolute;
  bottom: 0;
  width: 40%;
  left: 80%;
  align-self:flex-end;
  height: 2.5rem;            /* Footer height */
}

@font-face {
  font-family: Cormorant;
  src: url('assets/fonts/Cormorant-VariableFont_wght.ttf')
}
</style>
