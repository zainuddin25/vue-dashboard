<template>
    <div class="w-full p-4 bg-white rounded-md shadow-md">
        <div class="flex justify-between items-center">
            <img :src="img" :alt="img" class="w-8 h-8" />
            <img src="/img/Meatballs_menu.svg" alt="dots" class="rotate-90 opacity-30 cursor-pointer" />
        </div>
        <div class="w-full my-2">
            <span class="text-sm text-gray-400">{{ desc }}</span>
        </div>
        <span class="text-4xl font-extrabold">{{ total }}</span>
        <span class="text-sm text-gray-400 pl-2">{{ title }}</span>
    </div>
</template>
  
<script setup>
import { defineProps } from 'vue'
  
const props = defineProps({
    total: {
      type: String,
      required: true
    },
    desc: {
      type: String,
      required: true
    },
    img: {
        type: String,
        required: true
    },
    title: {
        type: String,
        required: true
    }
})
</script>