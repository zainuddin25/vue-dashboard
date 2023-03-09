<template>
    <div class="mt-4 bg-white flex flex-col rounded-lg">
        <img :src="img" class="w-full rounded-lg" :alt="img" />
        <span class="font-bold pt-4 px-4 text-lg">{{ titleNews }}</span>
        <p class="font-normal pb-4 px-4 text-sm truncate">{{ newsDescription }}</p>
        <div class="flex justify-between items-center px-4 pb-4">
            <div class="flex flex-col">
                <span class="font-normal">{{ userCreated }}</span>
                <span class="text-sm">{{ dateCreated }}</span>
            </div>
            <NuxtLink to="/">    
                <button class="text-sm py-2 px-4 font-medium border border-black hover:bg-black bg-white hover:text-white rounded-md duration-300">
                    Detail
                </button>
            </NuxtLink>
        </div>
    </div>
</template>

<script setup>

import { defineProps } from 'vue';

const props = defineProps({
    img: {
        type: String,
        required: true
    },
    titleNews: {
        type: String,
        required: true
    },
    newsDescription: {
        type: String,
        required: true
    },
    userCreated: {
        type: String,
        required: true
    },
    dateCreated: {
        type: String,
        required: true
    }
})

</script>