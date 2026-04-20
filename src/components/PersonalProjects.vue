<template>
    <section>
        <div class="grid grid-cols-12 gap-1 w-[100vw] h-auto relative content-start left-[calc(50%-50vw)]">
            <div class="col-span-12 gap-10 text-[var(--element-color)] flex flex-row pl-3">
                <p class="ml-2 mt-1" style="font-size: 10px;">Source: Om mig</p>
                <p class="mt-1" style="font-size: 10px;">Effects controls</p>
                <RouterLink to="/about" class="mt-1" style="font-size: 10px;">Text</RouterLink>
                <p class="mt-1" style="font-size: 10px;">Properties</p>
                <RouterLink to="/school-projects" class="mt-1" style="font-size: 10px;">Project: Skole projekter
                </RouterLink>
                <RouterLink to="/personal-projects" class="mt-1"
                    style="font-size: 10px; text-decoration: underline; color: var(--text-color);">Project: Personlige
                    Projekter</RouterLink>
            </div>
            <h2 class="col-span-12 flex justify-center mt-10 mb-4 text-[var(--text-color)] font-bold"
                style="font-family: 'Mulish', sans-serif; font-size: 48px;">Personlige Projekter</h2>

            <!-- YouTube -->
            <div class="col-start-3 col-span-8 flex flex-col gap-10 w-full mb-10">
                <div class="h-auto bg-gradient-to-r to-[var(--background-color-dark)] from-[var(--background-color-bright)] w-full flex flex-col rounded">
                    <div class="flex flex-row-reverse w-full my-20">
                        <div class="w-1/2 h-auto flex flex-row justify-center items-center gap-5 p-10">
                            <div class="w-1/4 relative flex flex-col items-center">
                                <p class="text-[var(--text-color)] text-xl absolute -top-10 whitespace-nowrap">Klik her
                                </p>
                                <a href="https://www.youtube.com/@capfraiche" target="_blank" rel=""
                                    class="w-full flex items-center justify-center">
                                    <img src="../assets/yt-profile-picture.jpg" alt="YouTube Profile Picture"
                                        class="w-full rounded-full">
                                </a>
                            </div>
                            <p class="text-[var(--text-color)] font-bold pb-2" style="font-size: 48px;">+</p>
                            <img src="../assets/yt-logo.png" alt="YouTube logo" class="w-1/3 object-contain">

                        </div>
                        <div class="w-1/2 h-auto text-[var(--text-color)] flex">
                            <div class="w-3/4 h-auto flex flex-col ml-auto justify-center gap-3">
                                <h3 class="font-bold leading-none" style="font-size: 48px;">Youtube</h3>
                                <p>Jeg har siden Februar 2020 lavet Youtube videoer for sjovs skyld, med mig og mine
                                    kammeraters sjoveste øjeblikke</p>
                                <p>Siden da er jeg blevet bedre og bedre for hver video, da jeg har hver gang gået
                                    tilbage til den tidligere og kigget efter hvad jeg kunne have gjort bedre.</p>
                            </div>
                        </div>
                    </div>
                    <div class="flex flex-col h-auto w-full items-center pb-10 gap-5">
                        <div class="text-[var(--text-color)] text-center flex" style="width: calc(80% + 3.75rem); max-width: calc(64rem + 3.75rem);">
                            <p>Jeg er begyndt at lave små edits som intro til mine videoer, for at udfordre mig selv
                                mere i at holde styr på tempo, timing og design på samme tid.</p>
                        </div>
                        <div class="w-full h-auto mt-5 flex flex-row gap-15 px-5 justify-center">
                            <div class="w-[40%] max-w-lg flex flex-col items-center">
                                <div class="text-[var(--text-color)] text-center mb-3">
                                    <h4 class="font-bold text-xl leading-tight">DE TRE BJERGBESTIGERE</h4>
                                    <h4 class="font-bold text-xl leading-tight">[PEAK]</h4>
                                </div>
                                <div class="border-2 border-[#3d3d3d] w-full aspect-video rounded overflow-hidden">
                                    <iframe class="w-full h-full"
                                        src="https://www.youtube.com/embed/XG9ZFK5Q5Es?start=15"
                                        title="YouTube video player" frameborder="0"
                                        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                                        allowfullscreen>
                                    </iframe>
                                </div>
                                <p class="text-[var(--text-color)] text-xs mt-3">
                                    Klik <a href="https://youtu.be/XG9ZFK5Q5Es?si=Q2ogJGCaqXi7TJ6t" target="_blank"
                                        class="underline hover:text-blue-500 transition-colors">her</a>
                                    for at se hele videoen på YouTube.
                                </p>
                            </div>
                            <div class="w-[40%] max-w-lg flex flex-col items-center">
                                <div class="text-[var(--text-color)] text-center mb-3">
                                    <h4 class="font-bold text-xl leading-tight">UNDSLIP BAGLOKALERNE</h4>
                                    <h4 class="font-bold text-xl leading-tight">[ESCAPE THE BACKROOMS]</h4>
                                </div>
                                <div class="border-2 border-[#3d3d3d] w-full aspect-video rounded overflow-hidden">
                                    <iframe class="w-full h-full"
                                        src="https://www.youtube.com/embed/MpgyDM-VEdo?start=46"
                                        title="YouTube video player" frameborder="0"
                                        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                                        allowfullscreen>
                                    </iframe>
                                </div>
                                <p class="text-[var(--text-color)] text-xs mt-3">
                                    Klik <a href="https://youtu.be/MpgyDM-VEdo?si=eM083jpYr6Vmuvol" target="_blank"
                                        class="underline hover:text-blue-500 transition-colors">her</a> for at se hele
                                    videoen på YouTube.
                                </p>
                            </div>
                        </div>
                        <div class="w-full h-auto flex flex-col items-center mt-10 px-5">
                            <div class="w-[40%] max-w-lg flex flex-col items-center">
                                <div class="text-[var(--text-color)] text-center mb-3">
                                    <h4 class="font-bold text-xl leading-tight">DE TRE SKRALDESPANDE</h4>
                                    <h4 class="font-bold text-xl leading-tight">[R.E.P.O]</h4>
                                </div>
                                <div class="border-2 border-[#3d3d3d] w-full aspect-video rounded overflow-hidden">
                                    <iframe class="w-full h-full"
                                        src="https://www.youtube.com/embed/fYwX_U2IcsU?start=37"
                                        title="YouTube video player" frameborder="0"
                                        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                                        allowfullscreen>
                                    </iframe>
                                </div>
                                <p class="text-[var(--text-color)] text-xs mt-3">
                                    Klik <a href="https://youtu.be/fYwX_U2IcsU?si=WCM5f-ELzb91YCU-" target="_blank"
                                        class="underline hover:text-blue-500 transition-colors">her</a>
                                    for at se hele videoen på YouTube.
                                </p>
                            </div>
                        </div>
                        <div class="text-[var(--text-color)] justify-center flex text-center mt-16">
                            <p>Udover almindelige videoer med de bedste øjeblikke, har jeg også lavet videoer med webcam
                                og VR.</p>
                        </div>
                        <div class="w-full h-auto mt-5 flex flex-row gap-15 px-5 justify-center">
                            <div class="w-[40%] max-w-lg flex flex-col items-center">
                                <div class="text-[var(--text-color)] text-center mb-3">
                                    <h4 class="font-bold text-xl leading-tight">BLOD LATTER OG TÅRER</h4>
                                    <h4 class="font-bold text-xl leading-tight">[Chained Together]</h4>
                                </div>
                                <div class="border-2 border-[#3d3d3d] w-full aspect-video rounded overflow-hidden">
                                    <iframe class="w-full h-full"
                                        src="https://www.youtube.com/embed/mPierZicIVY?si=1qUzAML7paF6ABo7"
                                        title="YouTube video player" frameborder="0"
                                        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                                        allowfullscreen>
                                    </iframe>
                                </div>
                                <p class="text-[var(--text-color)] text-xs mt-3">
                                    Klik <a href="https://youtu.be/mPierZicIVY?si=1qUzAML7paF6ABo7" target="_blank"
                                        class="underline hover:text-blue-500 transition-colors">her</a>
                                    for at se hele videoen på YouTube.
                                </p>
                            </div>
                            <div class="w-[40%] max-w-lg flex flex-col items-center">
                                <div class="text-[var(--text-color)] text-center mb-3">
                                    <h4 class="font-bold text-xl leading-tight">RICK GRIMES LÆRLINGE</h4>
                                    <h4 class="font-bold text-xl leading-tight">[Arizona Sunshine 2 VR]</h4>
                                </div>
                                <div class="border-2 border-[#3d3d3d] w-full aspect-video rounded overflow-hidden">
                                    <iframe class="w-full h-full"
                                        src="https://www.youtube.com/embed/tR4f81Bz_Xw?si=ztbwpIsXub1omM1C"
                                        title="YouTube video player" frameborder="0"
                                        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                                        allowfullscreen>
                                    </iframe>
                                </div>
                                <p class="text-[var(--text-color)] text-xs mt-3">
                                    Klik <a href="https://youtu.be/tR4f81Bz_Xw?si=ztbwpIsXub1omM1C" target="_blank"
                                        class="underline hover:text-blue-500 transition-colors">her</a> for at se hele
                                    videoen på YouTube.
                                </p>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Photoshop -->
                <div class="h-auto bg-gradient-to-r from-[var(--background-color-dark)] to-[var(--background-color-bright)] w-full flex flex-col rounded">
                    <div class="flex flex-row w-full h-auto mt-10 mb-20 px-5 gap-15 justify-center items-center">
                        <div class="w-[40%] max-w-lg flex flex-col gap-10">
                            <img src="../assets/as-vr.jpg" alt=""
                                class="w-full border-2 border-[#3d3d3d] rounded overflow-hidden object-cover">
                                <img src="../assets/repo.jpg" alt=""
                                    class="w-full border-2 border-[#3d3d3d] rounded overflow-hidden object-cover">
                                <img src="../assets/sotf.jpg" alt=""
                                    class="w-full border-2 border-[#3d3d3d] rounded overflow-hidden object-cover">
                            </div>
                            <div class="w-[40%] max-w-lg h-auto text-[var(--text-color)] flex">
                                <div class="w-full h-auto flex flex-col ml-10 justify-center gap-3">
                                    <h3 class="font-bold leading-none" style="font-size: 48px;">Photoshop</h3>
                                    <p class="pr-30">Jeg laver mine egne thumbnails til hver video i Photoshop, da jeg
                                        ikke
                                        synes det er nok kun at udfordre mig selv i Premiere Pro.</p>
                                    <p class="pr-30">Her er tre af mange thumbnails jeg har lavet.</p>
                                </div>
                            </div>
                        </div>
                        <div
                            class="w-full h-auto my-10 flex flex-col items-center text-[var(--text-color)]">
                            <div class="text-center" style="width: calc(80% + 3.75rem); max-width: calc(64rem + 3.75rem);">
                                <p class="mb-2">Nu hvor man alligevel er i gang med at
                                    uddanne sig til Multimedie Designer. Kan man lige så godt have det sjovt med de
                                    programmer
                                    man har til rådighed.</p>
                                <p class="font-bold" style="text-decoration: underline;">Tryk på billedet for at se før-billedet</p>
                            </div>
                            <div class="w-full flex justify-center px-5">
                                <div class="w-full relative mt-10 transition-opacity duration-300" style="width: calc(80% + 3.75rem); max-width: calc(64rem + 3.75rem);">
                                    <img :src="isShowingBeforeJul ? julafterImg : julbeforeImg" alt="Jul before/after"
                                        class="w-full cursor-pointer border-2 border-[#3d3d3d] rounded overflow-hidden"
                                        @click="isShowingBeforeJul = !isShowingBeforeJul">
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
import julbeforeImg from '../assets/jule-billede-before.jpg';
import julafterImg from '../assets/jule-billede-after.jpg';

const isShowingBeforeJul = ref(true);
const isShowingBeforeBeatup = ref(true);
const isShowingBeforeRecipe = ref(true);
</script>

<style scoped></style>
