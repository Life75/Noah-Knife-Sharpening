<template>
    <div id="main" class="pt-10">
    <Instructions id="instructions" class="mt-10 "/>
    <Testimonals id="testimonals" class="pt-36"/>
    <FAQ class="pt-36"/>
    <ContactUs id="contactUs" class="pt-36 pb-5"/>
    <div class="flex-col text-center  justify-center  rounded-md p-1.5">
        <p>Made by Austyn Washington. Want a custom website like this?</p>
        <el-link href="https://awashington.notion.site/Hi-I-m-Austyn-fa6d777cd1a4409faf3fdd734b44cb03?pvs=4" type="primary" class="text">Contact me here</el-link>
    </div>

    </div>
</template>

<script setup lang="ts">
import Testimonals from './Testimonals.vue';
import Instructions from './Instructions.vue';
import FAQ from './FAQ.vue';
import ContactUs from './ContactUs.vue';
console.log("hello world")
</script>

<style>
</style>