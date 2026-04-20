<template>
    <section class="w-[100vw] h-auto min-h-[100px] relative left-[calc(50%-50vw)] flex flex-row border-t-2 border-black bg-[#1E1E1E]">
        <div class="w-3/4 border-r-2 border-black">
            <img :src="timelineUrl" alt="Timeline" class="w-full h-auto object-cover object-left" />
        </div>
        <div class="w-1/4 h-auto bg-blue-500">

        </div>
    </section>
</template>

<script setup>
import timelineUrl from '@/assets/timeline.svg';
</script>

<style scoped>

</style>
