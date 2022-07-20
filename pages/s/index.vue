<script setup>
const route = useRoute();

onBeforeMount (async () => {
    await navigateTo('/')
})
</script>

<template>
  <div>
    <h1 class="text-9xl">
      Ngak ada apa-apa disini
    </h1>
  </div>
</template>