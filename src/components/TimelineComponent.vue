<template>
    <section class="w-[100vw] h-auto min-h-[100px] relative left-[calc(50%-50vw)] flex md:flex-row flex-col border-t-2 border-black bg-[#1E1E1E]">
        <div class="md:w-3/4 w-full md:border-r-2 sm:border-b-2 border-black overflow-hidden ">
            <img :src="timelineUrl" alt="Timeline" class="w-[calc(100%+120px)] max-w-none -ml-[120px] md:w-full md:ml-0 h-auto object-cover object-left" />
        </div>
        <div class="md:w-1/4 sm:w-full h-auto">
            <div class="flex justify-center pt-3 text-[var(--text-color)] font-bold" style="font-family: 'Mulish', sans-serif; font-size: 38px;">
                Mine styrker
            </div>
            <div class="flex flex-row place-content-evenly h-auto items-center">
                <div class="flex flex-col items-center gap-2">
                    <p class="text-[var(--text-color)] pb-2 text-center">Video redigering</p>
                    <img src="../assets/video-redigering.png" alt="Video Redigering">
                </div>
                <div class="flex flex-col items-center gap-2">
                    <p class="text-[var(--text-color)] pb-2 text-center">Billede redigering</p>
                    <img src="../assets/billede-redigering.png" alt="Billede Redigering">
                </div>
                <div class="flex flex-col items-center gap-2">
                    <p class="text-[var(--text-color)] pb-2 text-center">Kode</p>
                    <img src="../assets/kode.png" alt="Kode">
                </div>
            </div>

        </div>
    </section>
</template>

<script setup>
import timelineUrl from '@/assets/timeline.svg';
</script>

<style scoped>

</style>
