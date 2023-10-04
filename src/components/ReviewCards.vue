<template>
    <div></div>
</template>

<script setup lang="ts">
import { defineProps } from 'vue';
const props = defineProps({
    name: {type: String, required: true},
    stars: {type: Number, required: true},
    date: {type: Date, required: true},

})
</script>

<style>
</style>