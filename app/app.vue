<template>
  <div>
    <Header />
    <Home
      :page="$router.currentRoute.value"
      v-if="$router.currentRoute.value.name ? $router.currentRoute.value.name?.toString()?.length < 10 : false"
    />
    <NuxtPage />
    <Footer />
  </div>
</template>

<script setup lang="ts">
import "~/styles/index.scss";
import Lenis from "@studio-freight/lenis";
import gsap from "gsap";
import ScrollTrigger from "gsap/ScrollTrigger";

const projName = ref(`WhatWhatGoodyDo?`);
const projDesc = ref(`fragments of my imagination exposed to the light`);
const projImg = ref(`https://cdn.whatwouldgoodydo.com/12-principles-of-animations.webp`);

const computedPageMeta = computed(() => {
  return {
    title: projName.value,
    meta: [
      { hid: "description", property: "description", content: projDesc.value },
      { hid: "og-type", property: "og:type", content: "website" },
      { hid: "og-title", property: "og:title", content: projName.value },
      { hid: "og-description", property: "og:description", content: projDesc.value },
      {
        hid: "og-image",
        property: "og:image",
        content: projImg,
      },
      { hid: "twitter-card", property: "twitter:card", content: "summary_large_image" },
      { hid: "twitter-title", property: "twitter:title", content: projName.value },
      { hid: "twitter-description", property: "twitter:description", content: projDesc.value },
      {
        hid: "twitter-image",
        property: "twitter:image",
        content: projImg,
      },
    ],
  };
});

useHead(computedPageMeta);

onMounted(() => {
  const lenis = new Lenis({
    lerp: 0.1,
  });

  lenis.on("scroll", ScrollTrigger.update);

  gsap.ticker.add((time) => {
    lenis.raf(time * 1000);
  });

  gsap.ticker.lagSmoothing(0);
});
</script>
