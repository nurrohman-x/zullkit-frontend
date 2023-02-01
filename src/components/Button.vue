<script>
import { RouterLink } from 'vue-router';

export default {
    components: {
        RouterLink
    },
    props: {
        text: {
            type: String,
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
    }
}
</script>

<template>
    <RouterLink :to="path" :class="className"
        class="px-8 py-3 text-base font-medium border border-transparent rounded-full md:py-2 hover:shadow">
        {{ text }}
    </RouterLink>
</template>