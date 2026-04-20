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
                <div class="col-start-3 col-span-8 flex flex-col gap-10 w-full mb-10">
                    <div class="h-auto bg-gradient-to-r from-[var(--background-color-dark)] to-[var(--background-color-bright)] w-full flex flex-row rounded">
                        <div class="w-1/2 h-auto">
                            <img src="../assets/get-forked-poster.png" alt="" class="w-full">

                        </div>
                        <div class="w-1/2 h-auto text-[var(--text-color)] flex">
                            <div class="w-3/4 h-auto flex flex-col ml-auto justify-center gap-3">
                                <h3 class="font-bold leading-none" style="font-size: 48px;">GET FORKED</h3>
                                <p class="pr-60">Lorem ipsum dolor sit amet consectetur adipiscing elit quisque faucibus ex sapien vitae pellentesque sem placerat in id cursus mi pretium tellus duis convallis tempus.</p>
                                <div>
                                    <p>Programmer brugt:</p>
                                    <ul class="list-disc pl-6">
                                        <li>Adobe Illustrator</li>
                                        <li>Adobe Photoshop</li>
                                        <li>Adobe Indesign</li>
                                    </ul>
                                </div>
                            </div>
                        </div>
                    </div>

                    <div class="h-auto bg-gradient-to-r to-[var(--background-color-dark)] from-[var(--background-color-bright)] w-full flex flex-row-reverse rounded">
                        <div class="w-1/2 h-auto flex justify-center">
                            <img src="../assets/mini-me.png" alt="" class="w-1/2 object-contain my-5">

                        </div>
                        <div class="w-1/2 h-auto text-[var(--text-color)] flex">
                            <div class="w-3/4 h-auto flex flex-col mr-auto justify-center gap-3 pl-32">
                                <h3 class="font-bold leading-none" style="font-size: 48px;">GET FORKED</h3>
                                <p class="pr-30">Lorem ipsum dolor sit amet consectetur adipiscing elit quisque faucibus ex sapien vitae pellentesque sem placerat in id cursus mi pretium tellus duis convallis tempus.</p>
                                <div>
                                    <p>Programmer brugt:</p>
                                    <ul class="list-disc pl-6">
                                        <li>Adobe Illustrator</li>
                                        <li>Adobe Photoshop</li>
                                        <li>Adobe Indesign</li>
                                    </ul>
                                </div>
                            </div>
                        </div>
                    </div>

                    <div class="h-auto bg-gradient-to-r from-[var(--background-color-dark)] to-[var(--background-color-bright)] w-full flex flex-row rounded">
                        <div class="w-1/2 h-auto">
                            <img src="../assets/get-forked-poster.png" alt="" class="w-full">

                        </div>
                        <div class="w-1/2 h-auto text-[var(--text-color)] flex">
                            <div class="w-3/4 h-auto flex flex-col ml-auto justify-center gap-3">
                                <h3 class="font-bold leading-none" style="font-size: 48px;">GET FORKED</h3>
                                <p class="pr-60">Lorem ipsum dolor sit amet consectetur adipiscing elit quisque faucibus ex sapien vitae pellentesque sem placerat in id cursus mi pretium tellus duis convallis tempus.</p>
                                <div>
                                    <p>Programmer brugt:</p>
                                    <ul class="list-disc pl-6">
                                        <li>Adobe Illustrator</li>
                                        <li>Adobe Photoshop</li>
                                        <li>Adobe Indesign</li>
                                    </ul>
                                </div>
                            </div>
                        </div>
                    </div>

                    <div class="h-auto bg-gradient-to-r to-[var(--background-color-dark)] from-[var(--background-color-bright)] w-full flex flex-row-reverse rounded">
                        <div class="w-1/2 h-auto flex justify-center">
                            <img src="../assets/mini-me.png" alt="" class="w-1/2 object-contain my-5">

                        </div>
                        <div class="w-1/2 h-auto text-[var(--text-color)] flex">
                            <div class="w-3/4 h-auto flex flex-col mr-auto justify-center gap-3 pl-32">
                                <h3 class="font-bold leading-none" style="font-size: 48px;">GET FORKED</h3>
                                <p class="pr-30">Lorem ipsum dolor sit amet consectetur adipiscing elit quisque faucibus ex sapien vitae pellentesque sem placerat in id cursus mi pretium tellus duis convallis tempus.</p>
                                <div>
                                    <p>Programmer brugt:</p>
                                    <ul class="list-disc pl-6">
                                        <li>Adobe Illustrator</li>
                                        <li>Adobe Photoshop</li>
                                        <li>Adobe Indesign</li>
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
</script>

<style scoped>

</style>
