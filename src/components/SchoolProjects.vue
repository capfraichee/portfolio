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

                    <div v-for="project in projects" :key="project.id" :class="[
                        'h-auto w-full flex rounded',
                        project.isReverse 
                            ? 'bg-gradient-to-r to-[var(--background-color-dark)] from-[var(--background-color-bright)] flex-row-reverse' 
                            : 'bg-gradient-to-r from-[var(--background-color-dark)] to-[var(--background-color-bright)] flex-row'
                    ]">
                        <div :class="project.imageContainerClass">
                            <img 
                                v-if="project.isInteractive"
                                :src="project.isShowingAlt ? project.altImage : project.image" 
                                :alt="project.title" 
                                :class="project.imageClass" 
                                @click="project.isShowingAlt = !project.isShowingAlt">
                            <img 
                                v-else
                                :src="project.image" 
                                :alt="project.title" 
                                :class="project.imageClass">
                        </div>
                        <div class="w-1/2 h-auto text-[var(--text-color)] flex">
                            <div :class="project.textContainerClass">
                                <h3 class="font-bold leading-none sm:text-[24px] md:text-[48px]">{{ project.title }}</h3>
                                <p v-for="(paragraph, index) in project.paragraphs" :key="index" :class="project.pClass">{{ paragraph }}</p>
                                <p v-if="project.interactiveText" :class="[project.pClass, 'font-bold']" style="text-decoration: underline;">{{ project.interactiveText }}</p>
                                <div>
                                    <p>Programmer brugt:</p>
                                    <ul class="list-disc pl-6">
                                        <li v-for="(program, index) in project.programs" :key="index">{{ program }}</li>
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

import getForkedImg from '../assets/get-forked-poster.png';
import miniMeImg from '../assets/mini-me.png';
import beatupbeforeImg from '../assets/beat-up-before.png';
import beatupafterImg from '../assets/beat-up-after.PNG';
import recipesiteImg from '../assets/recipe-site.svg';
import recipecodeImg from '../assets/recipe-code.svg';

const projects = ref([
  {
    id: 1,
    title: 'GET FORKED',
    paragraphs: [
      'Vi fik til opgave at lave en plakat til skolens “International Day”.',
      'Jeg lavede en plakat inspireret af “Scream”-filmserien, hvor kniven er erstattet med en gaffel.'
    ],
    programs: ['Adobe Illustrator', 'Adobe Photoshop', 'Adobe InDesign'],
    image: getForkedImg,
    isReverse: false,
    imageContainerClass: 'w-1/2 h-auto',
    imageClass: 'w-full',
    textContainerClass: 'w-3/4 h-auto flex flex-col ml-auto justify-center gap-3',
    pClass: 'md:pr-60 sm:pr-10 sm:text-[14px] md:text-[16px]'
  },
  {
    id: 2,
    title: 'MINI-ME',
    paragraphs: [
      'En simpel, men effektiv designopgave, hvor vi skulle lave et miniaturebillede af os selv.',
      'Jeg syntes, det kunne være sjovt at lave mig selv som en Simpsons-figur, fordi jeg så rigtig meget Simpsons som barn.'
    ],
    programs: ['Adobe Illustrator'],
    image: miniMeImg,
    isReverse: true,
    imageContainerClass: 'w-1/2 h-auto flex justify-center',
    imageClass: 'w-1/2 object-contain my-5',
    textContainerClass: 'w-3/4 h-auto flex flex-col md:mr-auto justify-center gap-3 pl-23 md:pl-40 sm:w-full md:w-100',
    pClass: 'md:pr-10 sm:pr-0 sm:text-[14px] md:text-[16px]'
  },
  {
    id: 3,
    title: 'BEAT-UP FACE',
    paragraphs: [
      'Et Photoshop-projekt, hvor vi skulle redigere vores ansigter, så de så “beat up” ud.',
      'Jeg besluttede at gå all-in og gøre det så realistisk som muligt.'
    ],
    interactiveText: 'Tryk på billedet for at se før-billedet',
    programs: ['Adobe Photoshop'],
    image: beatupafterImg,
    altImage: beatupbeforeImg,
    isInteractive: true,
    isShowingAlt: false,
    isReverse: false,
    imageContainerClass: 'w-1/2 h-auto',
    imageClass: 'w-full cursor-pointer transition-opacity duration-300',
    textContainerClass: 'w-3/4 h-auto flex flex-col ml-auto justify-center gap-3',
    pClass: 'md:pr-60 sm:pr-10 sm:text-[14px] md:text-[16px]'
  },
  {
    id: 4,
    title: 'RECIPE SITE',
    paragraphs: [
      'En hjemmeside, vores underviser havde designet, som vi skulle genskabe. Vores eneste opgave var derfor at kode den i Visual Studio Code.'
    ],
    interactiveText: 'Tryk på billedet for at se en del af koden.',
    programs: ['Visual Studio Code'],
    image: recipesiteImg,
    altImage: recipecodeImg,
    isInteractive: true,
    isShowingAlt: false,
    isReverse: true,
    imageContainerClass: 'w-1/2 h-auto',
    imageClass: 'w-full cursor-pointer transition-opacity duration-300',
    textContainerClass: 'w-3/4 h-auto flex flex-col ml-auto justify-center gap-3',
    pClass: 'md:pr-60 sm:pr-10 sm:text-[14px] md:text-[16px]'
  },
]);
</script>

<style scoped>

</style>
