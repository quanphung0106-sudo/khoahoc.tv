<template>
    <div>
        <header class="shadow-sm bg-white">
            <nav class="container mx-auto p-4 flex justify-between">
                <NuxtLink to="/" class="font-bold">Project</NuxtLink>
                <ul class="flex gap-4">
                    <li>
                        <NuxtLink to="/">Home Page</NuxtLink>

                    </li>
                    <li>
                        <NuxtLink to="/about">About Page</NuxtLink>

                    </li>
                    <li class="btn">
                        <NuxtLink to="/products">Product Page</NuxtLink>
                    </li>
                </ul>
            </nav>
        </header>

        <!-- output the page content -->
        <div class="container mx-auto p-4">
            <slot />
        </div>
    </div>
</template>

<style scoped>
.router-link-exact-active {
    color: green
}
</style>