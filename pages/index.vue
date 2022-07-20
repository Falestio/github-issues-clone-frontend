<script setup>

const showForm = ref(false)

</script>

<template>
    <div class="p-4">
        <img src="~/assets/img/keset-welcom.jpg" class="mx-auto mb-4" alt="Selamat datang guys" width="200">
        <h1 class="text-4xl text-center">Welcome to forum app</h1>


        <div class="card-wrapper flex flex-col gap-4 mx-auto px-2 mt-8">
            <button class="bg-orange-500 text-white p-2 rounded block" @click="showForm = !showForm">Create Space</button>
            
            <form class="bg-white flex flex-col" v-show="showForm"> 
                <input placeholder="Space Name" type="text" name="space-name" id="space-name">
                <input placeholder="Space Description" type="text" name="space-description" id="space-description">
                <button class="bg-orange-500 text-white p2 rounded">Create</button>            
            </form>
            
            <NuxtLink to="/s/trackmania">
                <div class="p-6 rounded border-4 border-orange-600">
                    <div class="flex flex-col">
                        <h2 class="text-3xl text-orange-400">Trackmania</h2>
                        <p class="text-xl">
                            Lorem ipsum dolor, sit amet consectetur 
                            adipisicing elit. Ea, dignissimos minus
                            praesentium delectus quaerat repudiandae iusto
                            voluptates perferendis id quod? Quo voluptatum assumenda 
                            quae dolor magnam delectus dolorum rerum omnis.
                        </p>
                    </div>
                </div>
            </NuxtLink>
        </div>

    </div>



</template>

<style lang="postcss" scoped>
.card-wrapper {
    max-width: 765px;
}

input {
    @apply p-4 rounded border-2 border-gray-200 
}
</style>