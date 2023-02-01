<script setup>
import Logo from './Logo.vue';
import NavLink from './NavLink.vue';
import Button from '../Button.vue'; 
</script>

<template>
    <nav class="bg-white border-gray-200 px-2 sm:px-4 py-2.5 rounded dark:bg-gray-800">
        <div class="container flex flex-wrap items-center justify-between mx-auto my-2">
            <Logo />
            <div class="md:order-2">
                <Button text="Login" path="/login"
                    className="mr-2 text-black bg-gray-200 hover:bg-gray-300 md:text-sm md:px-8" />
                <Button text="Register" path="/register"
                    className="text-white bg-navy hover:bg-navy md:text-sm md:px-8" />
            </div>
            <NavLink />
        </div>
    </nav>
</template>