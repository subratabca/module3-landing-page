<script setup>
import { reactive } from 'vue';
import bigimage from "../assets/demo-screen.mp4";


const items = reactive([
    {
      id: 1,
      title: "Device Mockups",
      description: "Ready to use HTML/CSS device mockups, no Photoshop required!",
      icon:"bi-phone"
    },
    {
      id: 2,
      title: "Flexible Use",
      description: "Put an image, video, animation, or anything else in the screen!",
      icon:"bi-camera"
    },
    {
      id: 3,
      title: "Free to Use",
      description: "As always, this theme is free to download and use for any purpose!",
      icon:"bi-gift"
    },
    {
      id: 4,
      title: "Open Source",
      description: "Since this theme is MIT licensed, you can use it commercially!",
      icon:"bi-patch-check"
    }
  ]);

</script>

<template>
        <section id="features">
            <div class="container px-5">
                <div class="row gx-5 align-items-center">
                    <div class="col-lg-8 order-lg-1 mb-5 mb-lg-0">
                        <div class="container-fluid px-5">
                            <div class="row gx-5">
                                <div class="col-md-6 mb-5" v-for="(item,index) in items" :key="item.id">
                                    <!-- Feature item-->
                                    <div class="text-center">
                                        <i class="icon-feature text-gradient d-block mb-3" :class="items[index].icon"></i>
                                        <h3 class="font-alt">{{ item.title }}</h3>
                                        <p class="text-muted mb-0">{{ item.description }}</p>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="col-lg-4 order-lg-0">
                        <!-- Features section device mockup-->
                        <div class="features-device-mockup">
                            <svg class="circle" viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg">
                                <defs>
                                    <linearGradient id="circleGradient" gradientTransform="rotate(45)">
                                        <stop class="gradient-start-color" offset="0%"></stop>
                                        <stop class="gradient-end-color" offset="100%"></stop>
                                    </linearGradient>
                                </defs>
                                <circle cx="50" cy="50" r="50"></circle></svg
                            ><svg class="shape-1 d-none d-sm-block" viewBox="0 0 240.83 240.83" xmlns="http://www.w3.org/2000/svg">
                                <rect x="-32.54" y="78.39" width="305.92" height="84.05" rx="42.03" transform="translate(120.42 -49.88) rotate(45)"></rect>
                                <rect x="-32.54" y="78.39" width="305.92" height="84.05" rx="42.03" transform="translate(-49.88 120.42) rotate(-45)"></rect></svg
                            ><svg class="shape-2 d-none d-sm-block" viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg"><circle cx="50" cy="50" r="50"></circle></svg>
                            <div class="device-wrapper">
                                <div class="device" data-device="iPhoneX" data-orientation="portrait" data-color="black">
                                    <div class="screen bg-black">
                                        <!-- PUT CONTENTS HERE:-->
                                        <!-- * * This can be a video, image, or just about anything else.-->
                                        <!-- * * Set the max width of your media to 100% and the height to-->
                                        <!-- * * 100% like the demo example below.-->
                                        <video muted="muted" autoplay="" loop="" style="max-width: 100%; height: 100%"><source :src="bigimage" type="video/mp4" /></video>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>
</template>

<style scoped>

</style>