<script setup>
    const route = useRoute()

    const currRoute = route.params.question

    const showForm = ref(false)
</script>

<template>
    <div>
        <div class="con pt-8">
            <h1 class="text-4xl">Bagiamana cara melakukan slidebug</h1>
            <hr class="mt-4">
            <div class="flex flex-col mt-8">
                <div class="p-2 flex justify-between items-center border-2 border-orange-500">
                    <div>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Sapiente, aspernatur illum fugit sed nostrum, omnis atque doloremque a tempore praesentium earum soluta nesciunt beatae quasi magni vero magnam ex qui necessitatibus dolorum nisi provident numquam. Provident eius ipsam facere est natus quas voluptate, minima nihil dignissimos eveniet tempora inventore unde!</p>
                        <p class="text-sm">Diposting 4 jam yang lalu oleh barjasanjaya</p>
                    </div>
                </div>

                <button class="text-white p-2 rounded" @click="showForm = !showForm">Create Space</button>
            
                <form class="bg-white flex flex-col" v-show="showForm"> 
                    <input placeholder="Response" type="text" name="response" id="response">
                    <button class="bg-orange-500 text-white p2 rounded">Create</button>            
                </form>
            </div>
        </div>
    </div>
</template>