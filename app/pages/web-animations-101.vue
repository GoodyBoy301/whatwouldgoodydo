<template>
  <main class="playlist">
    <LiteYouTubeEmbed id="YnrsHLPxBAE" title="Part 1 | Web Animations 101 | How Web Animation Actually Works (CPU vs GPU)" />
  </main>
</template>

<script setup lang="ts">
import LiteYouTubeEmbed from "vue-lite-youtube-embed";
import "vue-lite-youtube-embed/style.css";

const projName = ref(`Web Animations 101`);
const projDesc = ref(`What would Goody do?`);
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
</script>
