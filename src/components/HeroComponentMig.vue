<template>
    <section class="mt-[70px]">
        <div class="flex flex-row w-[100vw] h-50 relative left-[calc(50%-50vw)]">
            <div class="h-50 flex-1 border-r-[2px] border-black flex flex-row gap-10 text-[var(--element-color)]">
                <p class="ml-2 mt-1" style="font-size: 10px;">Source: Om mig</p>
                <p class="mt-1" style="font-size: 10px;">Effects controls</p>
                <p class="mt-1" style="font-size: 10px; text-decoration: underline; color: var(--text-color);">Text</p>
                <p class="mt-1" style="font-size: 10px;">Properties</p>
                <RouterLink to="/school-projects" class="mt-1" style="font-size: 10px;">Project: Skole projekter</RouterLink>
                <RouterLink to="/personal-projects" class="mt-1" style="font-size: 10px;">Project: Personlige Projekter</RouterLink>
            </div>
            <div class="h-50 flex-1 text-[var(--element-color)] flex flex-row gap-10">
                <p class="ml-2 mt-1" style="font-size: 10px; text-decoration: underline; color: var(--text-color)">Program: Video CV</p>
                <p class="ml-2 mt-1" style="font-size: 10px;">Media Browser</p>
            </div>
        </div>
    </section>
</template>

<script setup>
</script>

<style scoped>
a {
    transition: none;
}
a:hover {
    color: inherit;
    background-color: transparent;
}
</style>
