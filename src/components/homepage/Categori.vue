<script setup>
import Card from './Card.vue';

defineProps({
    datas: {
        type: Array
    },
    title: {
        type: String
    },
    className: {
        type: String
    }
}) 
</script>

<template>
    <div class="container px-4 mx-auto my-16 md:px-12">
        <h2 class="mb-4 text-xl font-medium md:mb-0 md:text-lg">
            {{ title }}
        </h2>
        <div class="flex flex-wrap -mx-1 lg:-mx-4">
            <Card v-for="data in datas" :key="data.id" :title="data.text" :desc="data.desc" :path="data.path"
                :image="data.image" :className="className" />
        </div>
    </div>
</template>