<template>
    <div class="mt-7 max-w-sm mx-auto text-center card">
        <p class="mt-7 text-7xl font-bold">{{ error.statusCode }}</p>
        <p class="mt-7 text-6xl">OOOpsss...</p>
        <p class="mt-7">{{ error.message }}</p>
        <button class="btn my-8" @click="handlClearError">Go Home...</button>


    </div>
</template>

<script setup lang="ts">
defineProps(['error'])

const handlClearError = () => clearError({ redirect: "/" })
</script>

<style scoped>

</style>