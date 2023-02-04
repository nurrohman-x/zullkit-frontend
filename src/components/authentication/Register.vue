<script setup>
import { ref } from 'vue';
import Button from '../Button.vue';
import Input from '../Input.vue';

const formRegister = ref({
    name: '',
    email: '',
    password: ''
})
</script>

<template>
    <form>
        <div class="mb-4">
            <Input type="text" label="Full name" v-model="formRegister.name" />
        </div>
        <div class="mb-4">
            <Input type="email" label="Email" v-model="formRegister.email" />
        </div>
        <div class="mb-4">
            <Input type="password" label="Password" v-model="formRegister.password" />
        </div>
        <div class="mt-6">
            <Button text="Continue Sign Up" path="/login"
                className="inline-flex items-center justify-center w-full text-white bg-indigo-600 hover:bg-indigo-700 md:text-lg md:px-10" />
            <button type="button"
                class="inline-flex items-center justify-center w-full px-8 py-3 mt-2 text-base font-medium text-black bg-gray-200 border border-transparent rounded-full hover:bg-gray-300 md:py-2 md:text-lg md:px-10 hover:shadow">
                Sign In
            </button>
        </div>
    </form>
</template>