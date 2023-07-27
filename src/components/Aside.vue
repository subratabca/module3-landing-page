<script setup>
    import image from "../assets/tnw-logo.svg";
    const content = "An intuitive solution to a common problem that we all face, wrapped up in a single app!"
</script>

<template>
    <aside class="text-center bg-gradient-primary-to-secondary">
        <div class="container px-5">
            <div class="row gx-5 justify-content-center">
                <div class="col-xl-8">
                    <div class="h2 fs-1 text-white mb-4">{{ content }}</div>
                    <img :src="image" alt="..." style="height: 3rem" />
                </div>
            </div>
        </div>
    </aside>
</template>


<style scoped>

</style>