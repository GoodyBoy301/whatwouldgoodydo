<script setup lang="ts">
import gsap from "gsap";
import type { RouteLocationNormalizedGeneric } from "vue-router";
import content from "~/content";
import { motion } from "motion-v";
const props = defineProps<{ page: RouteLocationNormalizedGeneric }>();
onMounted(() => {});
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
</script>

<template>
  <main class="home">
    <section class="home-hero">
      <h1>{{ props.page.name === "index" ? "What Would Goody Do?" : props.page.name }}</h1>
      <p>*fragments of my imagination exposed to the light</p>
    </section>
    <section class="home-list">
      <AnimatePresence :initial="false">
        <NuxtLink
          v-for="(item, i) in content.all.filter((item) => (page.name === 'index' ? true : item.category === page.name))"
          :href="item.url"
          :key="item.title"
        >
          <motion.div
            :key="item.title"
            :style="{ '--deg': (360 / content.all.length) * i }"
            :initial="{ height: 0, opacity: 0 }"
            :animate="{ height: 'auto', opacity: 1 }"
            :exit="{ height: 0, opacity: 0 }"
            :transition="{ duration: 0.2, ease: 'easeOut' }"
          >
            <motion.li
              @mouseenter="onHover"
              @mousedown="onClick"
              :initial="{
                opacity: 0,
                y: -8,
                scale: 0.98,
                filter: 'blur(4px)',
              }"
              :animate="{
                opacity: 1,
                y: 0,
                scale: 1,
                filter: 'blur(0px)',
              }"
              :exit="{
                opacity: 0,
                y: 8,
                scale: 0.98,
                filter: 'blur(4px)',
              }"
              :transition="{ duration: 0.15, ease: 'easeOut' }"
            >
              <figure></figure>
              <h2>{{ item.title }}</h2>
              <h3>{{ item.title }}</h3>
              <aside></aside>
              <Arrow />
            </motion.li>
          </motion.div>
        </NuxtLink>
      </AnimatePresence>
    </section>
    <audio ref="hoverSound" src="/audio/audio_3ea541baea.wav"></audio>
    <audio ref="clickSound" src="/audio/audio_3ea541baec.wav"></audio>
  </main>
</template>
