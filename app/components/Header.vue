<template>
  <header class="header">
    <NuxtLink class="header-link" @mouseenter="onHover" @mousedown="onClick" href="/" data-text="Home">Home</NuxtLink>
    <i />
    <NuxtLink class="header-link" @mouseenter="onHover" @mousedown="onClick" href="/videos" data-text="Videos">Videos</NuxtLink>
    <NuxtLink class="header-link" @mouseenter="onHover" @mousedown="onClick" href="/writings" data-text="Writings">
      Writings
    </NuxtLink>
    <NuxtLink class="header-logo" data-desktop @mousedown="onClick" href="/" data-text="WWGD?">WWGD?</NuxtLink>
    <NuxtLink class="header-link" data-desktop @mouseenter="onHover" @mousedown="onClick" href="/talks" data-text="Talks"
      >Talks</NuxtLink
    >
    <NuxtLink class="header-link" data-desktop @mouseenter="onHover" @mousedown="onClick" href="/workshops" data-text="Workshops">
      Workshops
    </NuxtLink>
    <NuxtLink class="header-link" data-desktop @mouseenter="onHover" @mousedown="onClick" href="/courses" data-text="Courses">
      Courses
    </NuxtLink>
    <audio ref="hoverSound" src="/audio/audio_3ea541baeb.wav"></audio>
    <audio ref="clickSound" src="/audio/audio_3ea541baec.wav"></audio>
  </header>
</template>

<script setup lang="ts">
import gsap from "gsap";
import { ScrambleTextPlugin } from "gsap/all";

const hoverSound = ref<HTMLAudioElement | null>(null);
const clickSound = ref<HTMLAudioElement | null>(null);
function onHover() {
  if (!hoverSound.value) return;
  hoverSound.value.currentTime = 0;
  hoverSound?.value?.play();
}

function onClick() {
  if (!clickSound.value) return;
  clickSound.value.currentTime = 0;
  clickSound?.value?.play();
}

onMounted(() => {
  gsap.registerPlugin(ScrambleTextPlugin);
  const links = document.querySelectorAll<HTMLElement>(".header-link");
  links.forEach((link) => {
    link.onmouseenter = () => {
      gsap.to(link, { duration: 0.4, scrambleText: link.dataset.text });
    };
  });
});
</script>
