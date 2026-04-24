<template>
    <section>
        <div class="flex sm:flex-col md:flex-row w-[100vw] h-auto relative left-[calc(50%-50vw)]">
            <div class="h-auto flex-1 md:border-r-[2px] md:border-b-0 border-black sm:border-b-[2px] sm:border-r-0">
                <div class="pl-3">
                    <div class="gap-10 text-[var(--element-color)] flex flex-row">
                        <p class="ml-2 mt-1" style="font-size: 10px;">Source: Om mig</p>
                        <p class="mt-1" style="font-size: 10px;">Effects controls</p>
                        <RouterLink to="/about" class="mt-1"
                            style="font-size: 10px; text-decoration: underline; color: var(--text-color);">Text
                        </RouterLink>
                        <p class="mt-1" style="font-size: 10px;">Properties</p>
                        <RouterLink to="/school-projects" class="mt-1" style="font-size: 10px;">Project: Skole projekter
                        </RouterLink>
                        <RouterLink to="/personal-projects" class="mt-1" style="font-size: 10px;">Project: Personlige
                            Projekter</RouterLink>
                    </div>
                    <div class="mt-10 grid grid-cols-12">
                        <p class="ml-2 mt-1 text-[var(--text-color)] col-span-2" style="font-size: 10px;">Casper</p>
                        <div class="flex flex-col col-span-10 col-start-3 col-end-12">
                            <p class="mt-1 text-[var(--element-color)]" style="font-size: 10px;">00:00:00:00 -
                                00:00:05:17</p>
                            <p class="mt-1 text-[var(--text-color)]" style="font-size: 16px;">Hejsa! Mit navn er Casper
                                og det her er mit portfolio.</p>
                        </div>
                    </div>
                    <div class="mt-3 grid grid-cols-12">
                        <p class="ml-2 mt-1 text-[var(--text-color)] col-span-2" style="font-size: 10px;">Casper</p>
                        <div class="flex flex-col col-span-10 col-start-3 col-end-12">
                            <p class="mt-1 text-[var(--element-color)]" style="font-size: 10px;">00:00:06:34 -
                                00:00:11:56</p>
                            <p class="mt-1 text-[var(--text-color)]" style="font-size: 16px; line-height: 22px;">Jeg
                                specialiserer mig inden for video- og billedredigering, da jeg har haft en gnist for
                                content creation siden jeg var barn.</p>
                        </div>
                    </div>
                    <div class="mt-3 grid grid-cols-12">
                        <p class="ml-2 mt-1 text-[var(--text-color)] col-span-2" style="font-size: 10px;">Casper</p>
                        <div class="flex flex-col col-span-10 col-start-3 col-end-12">
                            <p class="mt-1 text-[var(--element-color)]" style="font-size: 10px;">00:00:13:43 -
                                00:00:23:16</p>
                            <p class="mt-1 text-[var(--text-color)]" style="font-size: 16px; line-height: 22px;">
                                Redigering for mig er ikke bare at klippe videoer sammen, men at skabe en oplevelse hvor
                                timing, lyd og klip går hånd i hånd.</p>
                        </div>
                    </div>
                    <div class="mt-3 grid grid-cols-12">
                        <p class="ml-2 mt-1 text-[var(--text-color)] col-span-2" style="font-size: 10px;">Casper</p>
                        <div class="flex flex-col col-span-10 col-start-3 col-end-12">
                            <p class="mt-1 text-[var(--element-color)]" style="font-size: 10px;">00:00:25:05 -
                                00:00:39:56</p>
                            <p class="mt-1 text-[var(--text-color)]" style="font-size: 16px; line-height: 22px;">På
                                grund min store interesse for at redigere har jeg derfor valgt at designe mit portfolio
                                i et layout inspireret af Adobe Premiere Pro.</p>
                        </div>
                    </div>
                    <div class="mt-3 grid grid-cols-12">
                        <p class="ml-2 mt-1 text-[var(--text-color)] col-span-2" style="font-size: 10px;">Casper</p>
                        <div class="flex flex-col col-span-10 col-start-3 col-end-12">
                            <p class="mt-1 text-[var(--element-color)]" style="font-size: 10px;">00:00:39:56 -
                                00:00:44:19</p>
                            <p class="mt-1 text-[var(--text-color)]" style="font-size: 16px; line-height: 22px;">Kig dig
                                omkring og udforsk mine projekter.</p>
                        </div>
                    </div>
                </div>
                <div class="w-full mt-20 border-t-[2px] border-black grid grid-cols-12 min-h-[250px]">
                    <p class="pl-5 mt-2 col-span-2"
                        style="font-size: 10px; text-decoration: underline; color: var(--text-color)">Info</p>

                    <div class="flex flex-row gap-10 col-start-3 col-end-12 mt-16 mb-16 justify-between items-start">
                        <div class="w-full flex justify-start text-[var(--text-color)]">
                            <div class="flex flex-col items-start">
                                <p class=" mb-2">Kontakt mig</p>
                                <p class="flex flex-row items-center gap-3 mt-2">
                                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24">
                                        <path fill="currentColor"
                                            d="M6.62 10.79c1.44 2.83 3.76 5.14 6.59 6.59l2.2-2.2c.27-.27.67-.36 1.02-.24c1.12.37 2.33.57 3.57.57c.55 0 1 .45 1 1V20c0 .55-.45 1-1 1c-9.39 0-17-7.61-17-17c0-.55.45-1 1-1h3.5c.55 0 1 .45 1 1c0 1.25.2 2.45.57 3.57c.11.35.03.74-.25 1.02z" />
                                    </svg>
                                    +45 6131 6499
                                </p>
                                <p class="flex flex-row items-center gap-3 mt-4">
                                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24">
                                        <g fill="currentColor">
                                            <path
                                                d="M22 7.535V17a3 3 0 0 1-2.824 2.995L19 20H5a3 3 0 0 1-2.995-2.824L2 17V7.535l9.445 6.297l.116.066a1 1 0 0 0 .878 0l.116-.066z" />
                                            <path
                                                d="M19 4c1.08 0 2.027.57 2.555 1.427L12 11.797l-9.555-6.37a3 3 0 0 1 2.354-1.42L5 4z" />
                                        </g>
                                    </svg>
                                    casras01@easv365.dk
                                </p>
                            </div>
                        </div>
                        <div
                            class="w-full h-full flex justify-between items-center flex-col text-[var(--text-color)] py-2">
                            <p class="text-center">Min LinkedIn</p>
                            <a href="https://www.linkedin.com/in/casperbachr/" target="" rel=""
                                class="flex items-center justify-center h-10">
                                <img src="../assets/linkedin_logo.svg" alt="LinkedIn" class="w-10">
                            </a>
                        </div>
                        <div
                            class="w-full h-full flex justify-between items-center flex-col text-[var(--text-color)] py-2">
                            <p class="text-center leading-tight">Download mit skrevne CV her</p>
                            <a href="/casper-rasmussen-cv.pdf" target="_blank" download="Casper Bach Rasmussen CV.pdf"
                                class="bg-[var(--element-white)] text-[var(--background-color-dark)] px-8 py-2 rounded h-10 flex items-center justify-center whitespace-nowrap"
                                style="font-family: 'Mulish', sans-serif; font-weight: 900;">
                                Download CV
                            </a>
                        </div>
                    </div>

                </div>
            </div>
            <div class="h-auto flex-1">
                <div class="text-[var(--element-color)] flex flex-row gap-10">
                    <p class="md:ml-2 mt-1" style="font-size: 10px; text-decoration: underline; color: var(--text-color)">
                        Program: Video CV</p>
                    <RouterLink to="/personal-projects" class="mt-1" style="font-size: 10px;">Media Browser</RouterLink>
                </div>
                <div class="w-full h-auto flex flex-col items-center">
                    <h1 class="justify-center flex pt-10 text-[var(--text-color)]"
                        style="font-family: 'Mulish', sans-serif; font-weight: 650; font-size: 36px;">Mit video CV</h1>
                    <iframe class="w-6/7 block aspect-video" src="https://www.youtube.com/embed/vJ8LX2eXj5U"
                        title="YouTube video player" frameborder="0"
                        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                        allowfullscreen>
                    </iframe>
                    <img src="../assets/play-tab.png" alt="" class="w-6/7">
                </div>
            </div>
        </div>
    </section>
</template>

<script setup>
</script>

<style scoped></style>
