<template>
  <div 
    v-if="isVisible"
    class="w-full bg-yellow-400 text-black text-center py-4 px-6 rounded-md shadow-md"
  >
    <p class="text-lg font-bold">
      ✈️ Honeymoon Notice 🌸
    </p>
    <p class="text-base mt-1">
      I will be out of the country on my honeymoon from 
      <span class="font-semibold">September 16th – October 20th</span>.
    </p>
    <p class="text-base mt-1">
      I'm sorry for the inconvenience, but I will be glad to meet your sharpening needs when I get home!
    </p>
  </div>
</template>

<script setup lang="ts">
import { ref, onMounted } from 'vue'

// Set the active date range
const startDate = new Date('2025-09-16T00:00:00')
const endDate = new Date('2025-10-20T23:59:59')

const isVisible = ref(false)

onMounted(() => {
  const today = new Date()
  isVisible.value = today >= startDate && today <= endDate
})
</script>

<style scoped>
div {
  transition: background-color 0.3s ease;
}
div:hover {
  background-color: #facc15; /* slightly darker yellow */
}
</style>
