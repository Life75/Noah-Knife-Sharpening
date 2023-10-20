<template>
     <div>
                <div class=" transition rounded-lg opacity-25 -inset-1"></div>
                <div
                  class="relative p-6  rounded-lg bg-[#3b3837]  bg-opacity-70 shadow-lg pb-10"
                >
                  <div class="flex items-center space-x-4 ">
                    <div>
                      <h3 class="text-xl font-semibold text-white ">{{ props.name }}</h3>
                      <div><el-rate v-model="props.stars" disabled /></div>
                    </div>
                  </div>
                  <p class="review-text pt-3">
                        {{ props.description }}
                  </p>
                </div>
    </div>
</template>

<script setup lang="ts">
import { defineProps } from 'vue';
const props = defineProps({
    name: {type: String, required: true},
    stars: {type: Number, required: true},
    description: {type: String, required: true}

})
</script>

<style>
.review-text {
  @apply leading-normal  text-base font-bold text-lg;
}
</style>