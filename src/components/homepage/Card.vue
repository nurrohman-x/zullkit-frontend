<script setup>
import { RouterLink } from 'vue-router';

defineProps({
    title: String,
    desc: String,
    image: String,
    path: String,
    className: String
})
</script>

<template>
    <div class="w-full px-1 my-1 md:w-1/2 lg:my-4 lg:px-4 " :class="className ? className : 'lg:w-1/4'">
        <div class="overflow-hidden border border-gray-200 rounded-xl">
            <RouterLink :to="'/product/' + path">
                <div class="m-4 overflow-hidden rounded-xl">
                    <img alt="Placeholder" class="block w-full h-auto" :src="'/src/assets/img/' + image" />
                </div>
            </RouterLink>

            <header class="px-4 mb-4 leading-tight">
                <h1 class="text-lg">
                    <RouterLink class="font-semibold text-black no-underline hover:underline" :to="'/product/' + path">
                        {{ title }}
                    </RouterLink>
                </h1>
                <span class="block text-sm font-light text-gray-500 no-underline">
                    {{ desc }}
                </span>
            </header>
        </div>
    </div>
</template>