<template>
    <div>
        <header>
            <NuxtLink to="/products">Nuxt</NuxtLink>
        </header>
        <div>
            <slot />
        </div>
        <footer>
            <ul>
                <li>
                    <NuxtLink to="/">HOME</NuxtLink>
                    <NuxtLink to="/about">About</NuxtLink>
                    <NuxtLink to="/products">Products</NuxtLink>
                </li>
            </ul>
        </footer>
    </div>
</template>

<script setup lang="ts">

</script>

<style scoped>
li {
    display: flex;
    gap: 30px;
}

.router-link-exact-active {
    color: #1edf38;
}
</style>