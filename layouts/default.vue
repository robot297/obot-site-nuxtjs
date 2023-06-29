<template>
    <div class="border-2">
        <title>A Website</title>
        <header class="shadow-sm bg-white dark:bg-black dark:text-white">
            <nav class="container mx-auto p-4 flex justify-between">
                <NuxtLink class="web-banner dark:dark-web-banner" to="/">Amanda & Alex Wedding</NuxtLink>
                <ul class="flex gap-4">
                    <li><NuxtLink to="/">Home</NuxtLink></li>
                    <li><NuxtLink to="/event_details">Event Details</NuxtLink></li>
                </ul>
            </nav>
        </header>
    </div>
    <div class="container mx-auto p-4">
        <slot/>
    </div>

    <footer class="shadow-sm bg-white dark:bg-black dark:text-white align-bottom">
        <div class="border-2">
            <nav class="container footer-container mx-auto p-4 flex justify-between">
                <NuxtLink to="/contact_us">Contact Us</NuxtLink><br/>
                <NuxtLink to="https://www.github.com">Link to Code</NuxtLink>
            </nav>
        </div>
    </footer>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>
    .router-link-exact-active{
        color: blueviolet;
    }

    .web-banner{
        color: orange;
    }

    .dark-web-banner{
        color: purple;
    }
</style>