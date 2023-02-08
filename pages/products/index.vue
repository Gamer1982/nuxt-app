<template>
    <div class="grid grid-cols-4 gap-5">
        <div v-for="p in products">
            <ProductCard :product="p" />
        </div>
    </div>
</template>

<script setup>
definePageMeta({
    layout: 'products'
})

const { data: products } = await useFetch('https://fakestoreapi.com/products')

useHead({
    title: 'Nuxt3 App | Merch',
    meta: [
        { name: 'description', content: 'Merch HA' }
    ],
    link: [
        {
            rel: 'stylesheet',
            href: 'https://fonts.googleapis.com/icon?family=Material+Icons'
        }
    ]
})
</script>

<style scoped>

</style>