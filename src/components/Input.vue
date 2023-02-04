<script setup>
defineProps({
    label: {
        type: [String, Boolean],
        default: false
    },
    type: {
        type: String,
        default: 'text'
    },
    modelValue: {
        type: [String, Number],
        default: ''
    }
})
</script>

<template>
    <label class="block mb-1" v-if="label" :for="label">{{ label }}</label>
    <input :placeholder="'Type your email ' + label" :id="label" :type="type" :value="modelValue"
        @input="$emit('update:modelValue', $event.target.value)"
        class="block w-full py-3 mt-2 border border-gray-300 rounded-full shadow-sm px-7 focus:border-indigo-300 focus:outline-none focus:ring focus:ring-indigo-200 focus:ring-opacity-50 disabled:bg-gray-100" />
</template>