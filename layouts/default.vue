<template>
    <div>
        <header class="shadow-sm bg-slate-400">
            <nav class="container mx-auto p-4 justify-between">
                <ul class="flex gap-4">

                    <li>
                        <NuxtLink to="/">HOME</NuxtLink>
                    </li>
                    <li>
                        <NuxtLink to="/about">About</NuxtLink>
                    </li>
                    <li class="btn">
                        <NuxtLink to="/products">Products</NuxtLink>
                    </li>
                </ul>
                <a href="/about">normal link -- about page</a>
            </nav>
        </header>
        <div class="container mx-auto p-4">
            <slot />
        </div>
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