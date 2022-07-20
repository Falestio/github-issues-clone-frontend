<script setup>
    const route = useRoute()

    const currRoute = route.params.spacename
</script>

<template>
    <div class="con pt-8">
        <h1 class="text-4xl text-orange-400">Trackmania</h1>

        <NuxtLink to="/s/trackmania/new-question">New Question</NuxtLink>

        <div class="flex flex-col mt-8">
            <NuxtLink to="/s/trackmania/bagaimana-cara-melakukan-slidebug">
                <div class="p-2 flex justify-between items-center border-2 border-orange-500">
                    <div>
                        <h2 class="text-xl font-bold">Bagiamana cara melakukan slidebug</h2>
                        <p class="text-sm">Diposting 4 jam yang lalu oleh barjasanjaya</p>
                    </div>
                    <div class="flex gap-2 items-center">
                        <p class="text-sm">12</p>
                        <i class='bx bx-comment'>Comment</i>
                    </div>
                </div>
            </NuxtLink>
        </div>
    </div>
</template>