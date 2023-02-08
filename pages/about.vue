<template>
    <div>
        <h2>about</h2>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Non consectetur modi aut at et quos atque culpa
            obcaecati eveniet aliquam.</p>
        <div>{{ data }}</div>
    </div>
</template>

<script setup lang="ts">
const data = await useFetch("/api/shop")

</script>

<style scoped>
h2 {
    margin-bottom: 20px;
    font-size: 36px;
}

p {
    margin: 20px 0;
}
</style>