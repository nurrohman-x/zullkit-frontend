<script setup>
import { ref } from 'vue';
import Button from '../Button.vue';
import Input from '../Input.vue';

const formLogin = ref({
    email: '',
    password: ''
})
</script>

<template>
    <form>
        <div class="mb-4">
            <Input type="email" label="Email" v-model="formLogin.email" />
        </div>
        <div class="mb-4">
            <Input type="password" label="Password" v-model="formLogin.password" />
        </div>
        <div class="mt-6">
            <button type="button"
                class="inline-flex items-center justify-center w-full px-8 py-3 text-base font-medium text-white bg-indigo-600 border border-transparent rounded-full hover:bg-indigo-700 md:py-2 md:text-lg md:px-10 hover:shadow">
                Sign In
            </button>
            <Button text="Create New Account" path="/register"
                className="inline-flex items-center justify-center w-full mt-2 text-black bg-gray-200 hover:bg-gray-300 md:text-lg md:px-10" />
        </div>
    </form>
</template>