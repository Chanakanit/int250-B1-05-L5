<script setup>
import { ref } from 'vue';
let isOpen = ref(false)
</script>

<template>
    <nav class="flex justify-between items-center h-14 m-4 lg:mx-32">
        <!-- Logo -->
         <div>
            <img src="../assets/logo.svg" alt="logo">
         </div>

         <!-- Desktop Menu -->
        <div class=" hidden ml-12 space-x-8 font-bold text-sm lg:flex lg:flex-1">
            <a href="#">Features</a>
            <a href="#">Pricing</a>
            <a href="#">Resources</a>
        </div>

        <!-- Action -->
        <div class=" hidden font-bold text-sm space-x-4 lg:flex">
            <button>Login</button>
            <button class=" bg-cyan-400 text-white px-4 py-2 rounded-full">Sign Up</button>
        </div>

        <!-- Hamburger -->
        <div class="lg:hidden w-10 h-full">
            <button class=" w-full h-full flex justify-center items-center" @click="isOpen = !isOpen">
                <div v-if="!isOpen" class="flex flex-col space-y-[3px]">
                    <div class=" w-6 h-[3px] bg-gray-400"></div>
                    <div class=" w-6 h-[3px] bg-gray-400"></div>
                    <div class=" w-6 h-[3px] bg-gray-400"></div>
                </div>
                <div v-else-if="isOpen" class="w-full h-full text-lg flex items-center justify-center text-gray-400">
                    X
                </div>
            </button>
        </div>
        <!-- Hamburger Open -->
        <div v-if="isOpen" class=" absolute top-15 right-4 w-2/3 z-99 flex flex-col items-center text-center bg-gray-300 md:w-1/2 lg:hidden">
            <div class=" flex flex-col py-4 space-y-2">
                <a href="#">Features</a>
                <a href="#">Pricing</a>
                <a href="#">Resources</a>
            </div>
            <hr class="w-full ">
            <div class=" flex flex-col py-4 space-y-2">
                <button>Login</button>
                <button>Sign Up</button>
            </div>
        </div>

        
    </nav>
</template>

<style scoped>

</style>