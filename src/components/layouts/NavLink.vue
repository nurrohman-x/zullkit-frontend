<script setup>
import { RouterLink } from 'vue-router';
import { reactive } from 'vue';

const menus = reactive([
    { id: '1', title: 'Home', path: '/' },
    { id: '2', title: 'Categories', path: '/categories' },
    { id: '3', title: 'Pricing', path: '/pricing' },
    { id: '4', title: 'Study Case', path: '#' },
])
</script>

<template>
    <div class="items-center justify-between hidden w-full md:flex md:w-auto md:order-1" id="mobile-menu-2">
        <ul class="flex flex-col mt-4 md:flex-row md:space-x-8 md:mt-0 md:text-sm md:font-regular">
            <li v-for="menu in menus" :key="menu.id">
                <RouterLink :to="menu.path"
                    class="block py-2 pl-3 pr-4 text-gray-700 border-b border-gray-100 hover:bg-gray-50 md:hover:bg-transparent md:border-0 md:hover:text-indigo-600 md:p-0 dark:text-gray-400 md:dark:hover:text-white dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-gray-700"
                    aria-current="page">
                    {{ menu.title }}
                </RouterLink>
            </li>
        </ul>
    </div>
</template>