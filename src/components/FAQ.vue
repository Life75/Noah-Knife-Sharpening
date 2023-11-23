<template>
    <div class="md:flex text-center flex-none  " id="faq">
        <span class="w-3/5 pr-10">
            <p class="text-5xl font-semibold lg:text-left ">FAQ</p>
            <p class="text-3xl pt-5 lg:text-left">Answers to some questions you might have.</p>
        </span>
        <span class="w-full">
            <div>
    

    <v-expansion-panels
      v-model="panel"
    >
      <v-expansion-panel style="background-color: #353332;">
        <v-expansion-panel-title><p class="md:text-3xl text-xl text-white font-extrabold">How do I drop off my items?</p>
            <template v-slot:actions>
                <v-icon large color="white" icon="mdi-plus">
                </v-icon>
            </template>
        </v-expansion-panel-title>
        <v-expansion-panel-text>
            <div class="text-white text-xl lg:text-left">
                <p>Choose an open locker slot to put your items in.</p>
                <p>Take out the lock in the locker.</p>
                <p>Put your items in.</p>
                <p>Lock the locker then spin the combination.</p>
            </div>
        </v-expansion-panel-text>
      </v-expansion-panel>
    </v-expansion-panels>



    <v-expansion-panels
      v-model="panel2"
      class="py-5"
    >
      <v-expansion-panel style="background-color: #353332;">
        <v-expansion-panel-title expand-icon="mdi-menu-down"><p class="font-extrabold md:text-3xl text-white text-xl">How do I pick up my items?</p>
            <template v-slot:actions>
                <v-icon large color="white" icon="mdi-plus">
                </v-icon>
            </template>
        </v-expansion-panel-title>
        <v-expansion-panel-text>
            
            <div class="text-white text-xl lg:text-left">
                <p>Input the code to the lock for the locker with your items in it that you will have received over text.</p>
                <p>Retrieve your items.</p>
                <p>If paying in cash or check, leave payment inside locker, and re-lock the locker.</p>
            </div>
        </v-expansion-panel-text>
      </v-expansion-panel>
    </v-expansion-panels>

    
    
    

  </div>

        </span>    
    </div>
    
</template>


<script setup lang="ts">
    import { ref } from 'vue';
    
    
    const panel = ref()
    const panel2 = ref()
    
</script>

<style>
</style>