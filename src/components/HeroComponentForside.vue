<template>
    <section>
        <div class="md:bg-white sm:bg-[var(--background-color-bright)] col-start-1 col-end-13 fixed inset-0 z-50 rounded-none md:relative md:inset-auto md:z-auto md:h-[calc(100vh-100px)] md:mt-[40px] md:rounded flex items-end justify-center overflow-hidden">
            <div class="absolute top-[5px] right-[3px] w-6 h-6 bg-red-500 text-white hidden md:flex items-center justify-center">
                <span class="text-[12px] font-bold leading-none select-none">X</span>
            </div>

            <div class="bg-[var(--background-color-bright)] w-full h-[calc(100%-35px)] flex items-end justify-center relative">
                <img src="../assets/premiere-logo.svg" alt="Adobe Premiere Pro Logo" class="absolute sm:top-0 md:top-4 left-6 h-16 w-auto">
                <div class="absolute md:top-8 sm:top-4 right-8 flex items-center gap-10 text-[var(--background-element-white)]">
                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 256 256"><path fill="currentColor" d="m228.24 219.76l-51.38-51.38a86.15 86.15 0 1 0-8.48 8.48l51.38 51.38a6 6 0 0 0 8.48-8.48M38 112a74 74 0 1 1 74 74a74.09 74.09 0 0 1-74-74"/></svg>
                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 1024 1024"><path fill="currentColor" d="M1024 320.496c0-35.344-28.654-64-63.998-64H850.754c28.272-27.888 46.368-64.447 46.368-109.472c0-55.44-31.84-115.664-121.216-115.664c-117.6 0-215.84 125.216-262 195.408c-46.192-70.176-147.44-195.392-265.024-195.392c-89.376 0-121.216 60.224-121.216 115.664c0 45.008 18.592 81.584 47.44 109.472H64.002c-35.344 0-64 28.656-64 64V512.08h64.56v416.56c0 35.344 28.655 64 64 64h767.68c35.343 0 64-28.656 64-64V512.064h63.76V320.496zM775.906 95.376c39.568 0 57.216 16.625 57.216 51.665c0 71.088-79.344 109.439-153.968 109.439H570.818c45.471-67.536 125.504-161.104 205.088-161.104m-527.025.001c79.6 0 162.655 93.568 208.127 161.088H348.64c-74.624 0-156.976-39.344-156.976-110.432c0-35.024 17.648-50.656 57.217-50.656m711.12 352.687h-416V320.496h416zm-896-127.568h416v127.568h-416zm64.56 191.568h351.44v416.56h-351.44zm767.696 416.56H544.001v-416.56h352.256z"/></svg>
                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><g fill="currentColor" fill-rule="evenodd" clip-rule="evenodd"><path d="M16 9a4 4 0 1 1-8 0a4 4 0 0 1 8 0m-2 0a2 2 0 1 1-4 0a2 2 0 0 1 4 0"/><path d="M12 1C5.925 1 1 5.925 1 12s4.925 11 11 11s11-4.925 11-11S18.075 1 12 1M3 12c0 2.09.713 4.014 1.908 5.542A8.99 8.99 0 0 1 12.065 14a8.98 8.98 0 0 1 7.092 3.458A9 9 0 1 0 3 12m9 9a8.96 8.96 0 0 1-5.672-2.012A6.99 6.99 0 0 1 12.065 16a6.99 6.99 0 0 1 5.689 2.92A8.96 8.96 0 0 1 12 21"/></g></svg>
                </div>
                <div class="bg-[var(--background-color-dark)] w-full h-[calc(100%-100px)] grid grid-cols-12">
                        <div class="mt-12 col-start-3 col-end-11">
                            <div class=" h-20 flex items-center border-b-3 border-[var(--background-color-bright)]">
                                <h1 class="md:text-3xl sm:text-2xl text-[var(--text-color)]">
                                    Welcome to Premiere!
                                </h1>
                            </div>
                            <h2 class="md:text-2xl sm:text-xl text-[var(--text-color)] mt-7">
                                Select a project to begin
                            </h2>
                            <div class="flex border-b-[3px] border-[var(--background-color-bright)]  mt-10 text-[var(--text-color)] font-normal text-[12px]">
                                <div class="w-5/12 md:pl-30 sm:pl-10">NAME</div>
                                <div class="w-3/12">TYPE</div>
                                <div class="w-3/12">RECENT</div>
                                <div class="w-1/12 text-right">SIZE</div>
                            </div>
                            <RouterLink to="/about" class="w-full h-15 flex items-center font-normal text-[12px] text-[var(--text-color)] ">
                                <div class="w-5/12">Om mig</div>
                                <div class="w-3/12">Premiere Project</div>
                                <div class="w-3/12">2 hours ago</div>
                                <div class="w-1/12 text-right">289 KB</div>
                            </RouterLink>
                            <RouterLink to="/school-projects" class="w-full h-15 flex items-center font-normal text-[12px] text-[var(--text-color)] ">
                                <div class="w-5/12">Skole projekter</div>
                                <div class="w-3/12">Premiere Project</div>
                                <div class="w-3/12">18 hours ago</div>
                                <div class="w-1/12 text-right">311 KB</div>
                            </RouterLink>
                            <RouterLink to="/personal-projects" class="w-full h-15 flex items-center font-normal text-[12px] text-[var(--text-color)] ">
                                <div class="w-5/12">Personlige projekter</div>
                                <div class="w-3/12">Premiere Project</div>
                                <div class="w-3/12">2 days ago</div>
                                <div class="w-1/12 text-right">217 KB</div>
                            </RouterLink>


                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script setup>
</script>

<style scoped>
a {
    color: var(--text-color);
    text-decoration: none;
    border-bottom: 3px solid var(--background-color-bright);
}

a:hover {
    background-color: var(--background-color-bright);
    color: var(--text-color);
}
</style>
