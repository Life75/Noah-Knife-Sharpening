<template>
    <div>
        <P class="text-5xl text-center pb-4">Testimonals</P>
        <section id="testimonies" class="">
    <div class="max-w-6xl mx-8 md:mx-10 lg:mx-20 xl:mx-auto">


  


        <div class="grid grid-cols-1 gap-6 sm:grid-cols-2 lg:grid-cols-3 lg:gap-8">


            <ul class="space-y-8">
           
               
                <li class=" leading-6">
                    <div class="relative group">
                        <div
                            class="absolute transition rounded-lg opacity-25 -inset-1 ">
                        </div><a href="https://twitter.com/kanyewest" class="cursor-pointer">
                            <div
                                class="relative p-6 space-y-6 leading-none rounded-lg bg-[#534C4C] ring-1 ring-gray-900/5">
                                <div class="flex items-center space-x-4">
                                    <div>
                                        <h3 class="text-lg font-semibold text-white">Zach H</h3>
                                        <div><el-rate
                                        v-model="value"
                                        disabled
                                        /></div>
                                    </div>
                                </div>
                                <p class="leading-normal text-gray-300 text-md font-bold">"Noah is excellent! My knives have never been sharper and he came to me! I 1000% endorse his work and fair prices. If you need a knife sharpener he should be #1 on your list."</p>
                            </div>
                        </a>
                    </div>
                </li>

            </ul>


            <ul class="hidden space-y-8 sm:block">
                <li class="text-sm leading-6">
                    <div class="relative group">
                        <div
                            class="absolute transition rounded-lg opacity-25 -inset-1  blur duration-400 group-hover:opacity-100 group-hover:duration-200">
                        </div><a href="https://twitter.com/paraga" class="cursor-pointer">
                            <div
                                class="relative p-6 space-y-6 leading-none rounded-lg bg-[#534C4C] ring-1 ring-gray-900/5">
                                <div class="flex items-center space-x-4">
                                    <div>
                                        <h3 class="text-lg font-semibold text-white"> Justice F</h3>
                                        <div><el-rate
                                        v-model="value"
                                        disabled
                                        /></div>
                                    </div>
                                </div>
                                <p class="leading-normal text-gray-300 text-md font-bold">"I just used this service. I'm very very satisfied. Noah's very nice and professional. He left my Shikomizue razor sharp and even notified me of a problem with my cane sword. Reasonably priced and professional. I will use him again."</p>
                            </div>
                        </a>
                    </div>
                </li>
          
              
               
            </ul>


            <ul class="hidden space-y-8 lg:block">
                <li class="text-sm leading-6">
                    <div class="relative group">
                        <div
                            class="absolute transition rounded-lg opacity-25 -inset-1  duration-400 group-hover:opacity-100 group-hover:duration-200">
                        </div><a href="https://twitter.com/satyanadella" class="cursor-pointer">
                            <div
                                class="relative p-6 space-y-6 leading-none rounded-lg bg-[#534C4C] ring-1 ring-gray-900/5">
                                <div class="flex items-center space-x-4">
                                    <div>
                                        <h3 class="text-lg font-semibold text-white">Josh E</h3>
                                        <div><el-rate
                                        v-model="value"
                                        disabled
                                        /></div>
                                    </div>
                                </div>
                                <p class="leading-normal text-gray-300 text-md font-bold">Incredible service. I dropped off 16 Wustoff knives to Noah earlier today and he had them done within 2 hours. These knives have never been sharper! Very quick, very efficient, and very well priced. I would recommend this service to anyone in the Pinellas area who needs their blades honed.</p>
                            </div>
                        </a>
                    </div>
                </li>
          

                 
             
            </ul>


        </div>
    </div>
</section>
    </div>
</template>


<script setup lang="ts">
import {ref } from 'vue'
const value = ref(5)
</script>