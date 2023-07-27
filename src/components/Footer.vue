<script setup>
    const title = "Your Website 2023. All Rights Reserved.";
    const privacy = "Privacy";
    const terms = "Terms";
    const faq = "FAQ";
</script>

<template>
    <footer class="bg-black text-center py-5">
        <div class="container px-5">
            <div class="text-white-50 small">
                <div class="mb-2">&copy; {{ title }}</div>
                <a href="#!">{{ privacy }}</a>
                <span class="mx-1">&middot;</span>
                <a href="#!">{{ terms }}</a>
                <span class="mx-1">&middot;</span>
                <a href="#!">{{ faq }}</a>
            </div>
        </div>
    </footer>
</template>

<style scoped>

</style>