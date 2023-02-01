<script setup>
import Register from '../components/authentication/Register.vue';
import Costomizable from '../components/icon/Layer.vue';
import Badge from '../components/icon/Badge.vue'
import Book from '../components/icon/Book.vue'
</script>

<template>
    <div class="relative overflow-hidden bg-white">
        <div class="mx-auto">
            <div class="flex flex-col items-center w-full min-h-screen pt-6 sm:justify-center sm:pt-0">
                <div class="w-full p-5 mx-auto md:max-w-4xl">
                    <h2 class="mb-10 text-5xl font-bold text-center">
                        <span class="block lg:mb-2">Join & Get Our</span>
                        <span class="block">Pro Benefits</span>
                    </h2>
                </div>
                <div class="w-full p-5 mx-auto md:max-w-4xl">
                    <div class="grid grid-cols-1 gap-4 md:grid-cols-2">
                        <div class="mx-auto md:mx-0">
                            <div class="mb-12">
                                <div class="block mb-2">
                                    <Costomizable />
                                    <h3 class="inline-block ml-2 text-lg font-semibold">
                                        Customizable
                                    </h3>
                                </div>
                                <p class="mt-2 text-lg text-gray-500">
                                    Accelerate your work with our millions <br>
                                    of ready-to-use design projects.
                                </p>
                            </div>
                            <div class="mb-12">
                                <div class="block mb-2">
                                    <Badge />
                                    <h3 class="inline-block ml-2 text-lg font-semibold">
                                        500 Fortune
                                    </h3>
                                </div>
                                <p class="mt-2 text-lg text-gray-500">
                                    Accelerate your work with our millions <br>
                                    of ready-to-use design projects.
                                </p>
                            </div>
                            <div class="mb-12">
                                <div class="block mb-2">
                                    <Book />
                                    <h3 class="inline-block ml-2 text-lg font-semibold">
                                        Documentation
                                    </h3>
                                </div>
                                <p class="mt-2 text-lg text-gray-500">
                                    Accelerate your work with our millions <br>
                                    of ready-to-use design projects.
                                </p>
                            </div>
                        </div>
                        <div>
                            <Register />
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>