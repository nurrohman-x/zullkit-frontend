<script setup>
import { RouterLink } from 'vue-router';

defineProps({
    text: {
        type: [String, Number],
        default: ''
    },
    className: {
        type: String,
        default: ''
    },
    path: {
        type: String,
        required: true
    }
})
</script>

<template>
    <RouterLink :to="path" :class="className"
        class="px-8 py-3 text-base font-medium border border-transparent rounded-full md:py-2 hover:shadow">
        {{ text }}
    </RouterLink>
</template>