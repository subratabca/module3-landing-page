<script setup>
    import image from "../assets/google-play-badge.svg";
    import image1 from "../assets/app-store-badge.svg";
    const title = "Get the app now!"
</script>

<template>
        <section class="bg-gradient-primary-to-secondary" id="download">
            <div class="container px-5">
                <h2 class="text-center text-white font-alt mb-4">{{ title }}</h2>
                <div class="d-flex flex-column flex-lg-row align-items-center justify-content-center">
                    <a class="me-lg-3 mb-4 mb-lg-0" href="#!"><img class="app-badge" :src="image" alt="..." /></a>
                    <a href="#!"><img class="app-badge" :src="image1" alt="..." /></a>
                </div>
            </div>
        </section>
</template>

<style scoped>

</style>