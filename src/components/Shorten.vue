<script setup>
defineProps({
    links: Array
})
</script>

<template>
    <div class="relative">
        <div class="relative z-10 bg-blue-950 m-4 flex flex-col 
              p-8 pb-12 items-center justify-center text-center 
              space-y-4 rounded-sm -mt-10 
              md:p-10 md:flex-row md:space-y-0 md:space-x-2 
              md:mx-auto max-w-screen-md">
            <input type="text" placeholder="Shorten a link here" class=" placeholder:text-amber-300 bg-white p-2 w-full h-10 rounded-lg md:flex-3">
            <button class=" bg-cyan-500 w-full py-2 rounded-lg text-white md:flex-1">Shorten It!</button>
        </div>
        <div class=" bg-gray-200 relative -mt-30 pt-4 pb-4 md:-mt-15">
            <div class="mt-30 space-y-4 md:mt-15 mx-auto  max-w-screen-md">
                <div v-for="value in links" class="mx-4 flex flex-col items-center text-center bg-white space-y-2 py-6 px-6 md:flex-row md:space-y-0 md:space-x-4 lg:mx-0">
                    <p class=" font-bold text-sm">{{ value.original }}</p>
                    <p class=" text-cyan-500 text-sm md:flex-1 md:text-right">{{ value.short }}</p>
                    <button class=" bg-cyan-500 text-sm text-white py-1 px-4 rounded-sm" :class="value.isFocus ? 'bg-cyan-950' : ''">Copy</button>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped></style>