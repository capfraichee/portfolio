<template>
    <section>
        <div class="grid grid-cols-12 gap-1 w-[100vw] h-auto relative content-start left-[calc(50%-50vw)]">
            <div class="col-span-12 gap-10 text-[var(--element-color)] flex flex-row pl-3">
                <p class="ml-2 mt-1" style="font-size: 10px;">Source: Om mig</p>
                <p class="mt-1" style="font-size: 10px;">Effects controls</p>
                <RouterLink to="/about" class="mt-1" style="font-size: 10px;">Text</RouterLink>
                <p class="mt-1" style="font-size: 10px;">Properties</p>
                <RouterLink to="/school-projects" class="mt-1" style="font-size: 10px; text-decoration: underline; color: var(--text-color);">Project: Skole projekter</RouterLink>
                <RouterLink to="/personal-projects" class="mt-1" style="font-size: 10px;">Project: Personlige Projekter</RouterLink>
            </div>
            <h1 class="col-span-12 flex justify-center mt-10 mb-4 text-[var(--text-color)] font-bold" style="font-family: 'Mulish', sans-serif; font-size: 48px;">Skole Projekter</h1>
                <div class="md:col-start-3 md:col-span-8 col-span-12 flex flex-col gap-10 mb-10 sm:px-10 md:px-0 md:px-0">

                    <!-- Get Forked Poster -->
                    <div class="h-auto bg-gradient-to-r from-[var(--background-color-dark)] to-[var(--background-color-bright)] w-full flex flex-row rounded">
                        <div class="w-1/2 h-auto">
                            <img src="../assets/get-forked-poster.png" alt="" class="w-full">
                        </div>
                        <div class="w-1/2 h-auto text-[var(--text-color)] flex">
                            <div class="w-3/4 h-auto flex flex-col ml-auto justify-center gap-3">
                                <h3 class="font-bold leading-none sm:text-[24px] md:text-[48px]">GET FORKED</h3>
                                <p class="md:pr-60 sm:pr-10 sm:text-[14px] md:text-[16px]">Vi fik til opgave at lave en plakat til skolens “International Day”.</p>
                                <p class="md:pr-60 sm:pr-10 sm:text-[14px] md:text-[16px]">Jeg lavede en plakat inspireret af “Scream”-filmserien, hvor kniven er erstattet med en gaffel.</p>
                                <div>
                                    <p>Programmer brugt:</p>
                                    <ul class="list-disc pl-6">
                                        <li>Adobe Illustrator</li>
                                        <li>Adobe Photoshop</li>
                                        <li>Adobe InDesign</li>
                                    </ul>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- Mini-me -->
                    <div class="h-auto bg-gradient-to-r to-[var(--background-color-dark)] from-[var(--background-color-bright)] w-full flex flex-row-reverse rounded">
                        <div class="w-1/2 h-auto flex justify-center">
                            <img src="../assets/mini-me.png" alt="" class="w-1/2 object-contain my-5">

                        </div>
                        <div class="w-1/2 h-auto text-[var(--text-color)] flex">
                            <div class="w-3/4 h-auto flex flex-col md:mr-auto justify-center gap-3 pl-23 md:pl-40 sm:w-full md:w-100">
                                <h3 class="font-bold leading-none text-[24px] md:text-[48px]">MINI-ME</h3>
                                <p class="md:pr-10 sm:pr-0 sm:text-[14px] md:text-[16px]">En simpel, men effektiv designopgave, hvor vi skulle lave et miniaturebillede af os selv.</p>
                                <p class="md:pr-10 sm:text-[14px] md:text-[16px]">Jeg syntes, det kunne være sjovt at lave mig selv som en Simpsons-figur, fordi jeg så rigtig meget Simpsons som barn.</p>
                                <div>
                                    <p>Programmer brugt:</p>
                                    <ul class="list-disc pl-6">
                                        <li>Adobe Illustrator</li>
                                    </ul>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- Beat-up face -->
                    <div class="h-auto bg-gradient-to-r from-[var(--background-color-dark)] to-[var(--background-color-bright)] w-full flex flex-row rounded">
                        <div class="w-1/2 h-auto">
                            <img 
                                :src="isShowingBeforeBeatup ? beatupafterImg : beatupbeforeImg" 
                                alt="Beat-up ansigt" 
                                class="w-full cursor-pointer transition-opacity duration-300" 
                                @click="isShowingBeforeBeatup = !isShowingBeforeBeatup">

                        </div>
                        <div class="w-1/2 h-auto text-[var(--text-color)] flex">
                            <div class="w-3/4 h-auto flex flex-col ml-auto justify-center gap-3">
                                <h3 class="font-bold leading-none sm:text-[24px] md:text-[48px]">BEAT-UP FACE</h3>
                                <p class="md:pr-60 sm:pr-10 sm:text-[14px] md:text-[16px]">Et Photoshop-projekt, hvor vi skulle redigere vores ansigter, så de så “beat up” ud.</p>
                                <p class="md:pr-60 sm:pr-10 sm:text-[14px] md:text-[16px]">Jeg besluttede at gå all-in og gøre det så realistisk som muligt.</p>
                                <p class="md:pr-60 sm:pr-10 sm:text-[14px] md:text-[16px] font-bold" style="text-decoration: underline;">Tryk på billedet for at se før-billedet</p>
                                <div>
                                    <p>Programmer brugt:</p>
                                    <ul class="list-disc pl-6">
                                        <li>Adobe Photoshop</li>
                                    </ul>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- Recipe site -->
                    <div class="h-auto bg-gradient-to-r to-[var(--background-color-dark)] from-[var(--background-color-bright)] w-full flex flex-row-reverse rounded">
                        <div class="w-1/2 h-auto">
                            <img 
                                :src="isShowingBeforeRecipe ? recipesiteImg : recipecodeImg" 
                                alt="Recipe site" 
                                class="w-full cursor-pointer transition-opacity duration-300" 
                                @click="isShowingBeforeRecipe = !isShowingBeforeRecipe">

                        </div>
                        <div class="w-1/2 h-auto text-[var(--text-color)] flex">
                            <div class="w-3/4 h-auto flex flex-col ml-auto justify-center gap-3">
                                <h3 class="font-bold leading-none sm:text-[24px] md:text-[48px]">RECIPE SITE</h3>
                                <p class="md:pr-60 sm:pr-10 sm:text-[14px] md:text-[16px]">En hjemmeside, vores underviser havde designet, som vi skulle genskabe. Vores eneste opgave var derfor at kode den i Visual Studio Code.</p>
                                <p class="md:pr-60 sm:pr-10 sm:text-[14px] md:text-[16px] font-bold" style="text-decoration: underline;">Tryk på billedet for at se en del af koden.</p>
                                <div>
                                    <p>Programmer brugt:</p>
                                    <ul class="list-disc pl-6">
                                        <li>Visual Studio Code</li>
                                    </ul>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
        </div>
    </section>
</template>

<script setup>
import { ref } from 'vue';

import beatupbeforeImg from '../assets/beat-up-before.png';
import beatupafterImg from '../assets/beat-up-after.PNG';
import recipesiteImg from '../assets/recipe-site.svg';
import recipecodeImg from '../assets/recipe-code.svg';

const isShowingBeforeBeatup = ref(true);
const isShowingBeforeRecipe = ref(true);
</script>

<style scoped>

</style>
