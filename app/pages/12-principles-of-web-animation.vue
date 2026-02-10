<template>
  <main class="article">
    <aside class="article-left">
      <NuxtLink href="#Preload" data-h2>1. Preload</NuxtLink>
      <NuxtLink href="#SmoothScroll" data-h2>2. Smooth Scroll</NuxtLink>
      <NuxtLink href="#CurateEmotions" data-h2>3. Curate Emotions</NuxtLink>
      <NuxtLink href="#Morph" data-h2>4. Morph</NuxtLink>
      <NuxtLink href="#Grace" data-h2>5. Grace</NuxtLink>
      <NuxtLink href="#Kinematics" data-h2>6. Kinematics</NuxtLink>
      <NuxtLink href="#Purpose" data-h2>7. Purpose</NuxtLink>
      <NuxtLink href="#Storytelling" data-h2>8. Storytelling</NuxtLink>
      <NuxtLink href="#Feedback" data-h2>9. Feedback</NuxtLink>
      <NuxtLink href="#Life" data-h2>10. Life</NuxtLink>
      <NuxtLink href="#Language" data-h2>11. Language</NuxtLink>
      <NuxtLink href="#Mimick" data-h2>12. Mimick</NuxtLink>
    </aside>
    <div class="article-right">
      <div class="article-head" id="Prologue">
        <h1>12 Principles of Web Animation</h1>
        <p>February 10, 2026</p>
        <p>Goodness Urama</p>
      </div>
      <div class="article-body">
        <p>
          If I had a system to create delightful web experiences, this would be my opinionated workflow, which I call the 12
          Principles of Web Animations.
        </p>
        <p>
          Before we begin, let's clarify what these terms mean. A web experience encompasses how a visitor feels, perceives, and
          engages with a brand during their entire visit. A positive experience is frictionless, intuitive, and occasionally
          immersive, helping users achieve their goals with ease, and at their core, web animations are simply animated/motion
          graphics on the web.
        </p>
        <p>
          While these principles have no specific interest in creating a positive experience, they are devoted to curating
          delightful and memorable ones through web animations.<br />
          These principles are essentially everything I know about motion, working with great designs, building for the web, and
          keeping those three elements in perfect synergy.
        </p>

        <h2 id="Preload">1 .{{ "  " }}Preload</h2>
        <div>
          <p>
            A delightful web experience starts even before anything loads, We need the size and roundtrips as minimal as possible,
            while prioritizing on a First Contentful Paint with no glitches. We also need to preload our heavier assets to make
            sure they are available as soon as they are needed.
          </p>
          <p>
            Loading times are critical and since we can't always guarantee a minimal load time (below 2s). We could use custom and
            engaging loaders, that require as little code and aseets as possible, to increase users' patience, reduce abandonment
            and tease what's behind the fold.
          </p>
          <p>
            We could also utilize file types/extensions optimized for the web like woff2, webp and webm, they enable us to have
            high-quality graphics with really small file sizes.<br />
            Caching all our data and preloading subsequent pages also ensures the navigation and whole experience are almost
            instant.
          </p>
          <b>
            A practical example is the preloader in the Jesus Website. Despite the progress not being accurately in sync with the
            load of the assets, it gives the assets more time to load, and initiates curiousity and excitement for the website
          </b>
          <video src="https://cdn.whatwouldgoodydo.com/video-sh292j.webm" muted loop playsinline />
        </div>

        <h2 id="SmoothScroll">2 .{{ "  " }}Smooth Scroll</h2>
        <div>
          <p>
            The Scroll is the Master Timeline of a web experience. A smooth scroll experience leverages the brain's visual
            processing system, helping users understand what's happening without needing to consume extensive text and graphics,
            while sustaining curiosity.
          </p>
          <p>
            We can use scrollytelling to bring content to life as it enters the viewport, using transforms, reveals and avoiding
            animating properties that are not GPU-accelerated to maintain a smooth and steady 60 fps. We also need to maintain
            consistency throughout the experience, create predictable patterns by using similar animations for similar
            interactions, and prioritize user control.
          </p>
          <p>
            We can't have animations everywhere though, when users become overwhelmed, animations lose their impact. We only need
            to add animations in places where they enrich the information and show relationships between elements or states.
          </p>
          <b>
            A practical example is the scroll in Deyemi The Actor, Highlighting a good story timeline, reveals and predictable
            patterns
          </b>
          <video src="https://cdn.whatwouldgoodydo.com/video-su18wn.webm" muted loop playsinline />
        </div>

        <h2 id="CurateEmotions">3 .{{ "  " }}Curate Emotions</h2>
        <div>
          <p>
            Our brains are naturally drawn to motion. We can harness this biological response to draw attention to important
            elements. However, this must be used carefully, as excessive or distracting animations can be annoying and pull users
            away from their primary task.
          </p>
          <p>
            Whenever possible, we need to give users unique experiences. Easter eggs are also a really good way to trigger
            positive emotions without affecting or hindering the rest of the website.
          </p>
          <p>
            When users feel something through an animation, it connects to their limbic system, which helps create memorable and
            engaging experiences. We can use animations to trigger pleasure, empathy, joy, and satisfaction and also chase away
            the negative emotions. We can reduce constant focus shifts by smoothly transitioning between different contexts,
            reduce anxiety by maintaining consistency and following intuitive conventions, and reduce cognitive overload by
            gracefully introducing new content.
          </p>
          <b>
            A practical example is the infinite scroll in the Nyatwa website. Might not even be the most memorable part of it, but
            it does trigger immense pleasure.
          </b>
          <video src="https://cdn.whatwouldgoodydo.com/video-uws8qa.webm" muted loop playsinline />
        </div>

        <h2 id="Morph">4 .{{ "  " }}Morph</h2>
        <div>
          <p>
            This principle involves animating elements as they change from one form or state to another, maintaining a visual
            connection to their origin. This minimizes the need for users to readjust mentally, helps them understand the
            relationship between different elements, conserves space, and sometimes simply adding extra delight.
          </p>

          <p>
            We can use seamless page transitions to maintain a sense of continuity, allowing users to see that elements are moving
            and changing rather than simply disappearing and reappearing. We leverage visual continuity by keeping shared elements
            visible and animating only their movement.
          </p>
          <p>
            We could approach complex animations by building out all elements and their potential states first. The animation then
            simply becomes a way to reveal or transform them over time.
          </p>
          <b>
            A practical example is the Payday Unboring Website. We maintain a single card throughout the experience, and transform
            this to fit into the the different screens and scenarios
          </b>
          <video src="https://cdn.whatwouldgoodydo.com/video-29abas.webm" muted loop playsinline />
        </div>

        <h2 id="Grace">5 .{{ "  " }}Grace</h2>
        <div>
          <p>
            Grace is simply smoothness and elegance in movement. A good animation should be invisible, not drawing undue attention
            to itself, graceful, interruptible, and should always respecting user preferences.
          </p>
          <p>
            The less work the browser has to do, the better the performance. If our animations are not smooth and performant, they
            end up playing a counterproductive role in the web experience.
          </p>
          <p>
            Interruptibility is the readiness for animations to be halted or rerouted instantly. Making sure our animations are
            always interruptible makes them feel more natural and responsive. We also need to ensure that if animations are
            disabled entirely and despite the type of device, users can still enjoy a full experience.
          </p>
          <b>
            A practical example is the mobile view of Payday Unboring Website, where we opted to forgo transitioning the card
            states to preserve performance without compromising the content.
          </b>
          <video src="https://cdn.whatwouldgoodydo.com/video-iiaao2.webm" muted loop playsinline />
        </div>

        <h2 id="Kinematics">6 .{{ "  " }}Kinematics</h2>
        <div>
          <p>
            This principle focuses on quantifying motion using position, displacement, velocity, and acceleration over time,
            without considering the forces causing them.
          </p>
          <p>
            Because nothing in the physical world changes instantly, when animating, we should generally start and end slowly,
            with acceleration in the middle, creating a more natural feel. This behavior is usually controlled by an easing curve
          </p>
          <p>
            Easing is by far the most important part of most animations. It is often the sole difference between a good, bad, or
            great animation. Mastering how to create, decide and use the right easing curves is a non-negotiable.
          </p>
          <p>
            We typically want to ease in and out for most animations happening on-screen, however, exceptions apply based on the
            element's origin and destination. When elements arrive from an unseen or void state, they are already moving so we
            ignore the ease in and simply ease out or decelerate to a stop, and when elements leave to an unseen or void state,
            they should not slow down before disappearing.
          </p>
          <b>
            A practical example is the features section in Onboard. For most of the motion, there's an ease-in-out, except the
            screens on the phone. Entering screens only ease-out and leaving screens only ease-in.
          </b>
          <video src="https://cdn.whatwouldgoodydo.com/video-58gds5.webm" muted loop playsinline />
        </div>

        <h2 id="Purpose">7 .{{ "  " }}Purpose</h2>
        <div>
          <p>
            Every animation must serve a clear goal, such as providing feedback, guiding user focus, explaining functionality, or
            enhancing storytelling. We need to keep animations brief and subtle to enhance, not overwhelm the experience.
            Distracting animations often feel like clumsy afterthoughts.
          </p>
          <p>
            Before adding any animation, we must consider how frequently users will see and interact with it. This principle
            dictates that we need to know when to add an animation, why, and when not to. The primary focus should always be on
            necessity and utility, ensuring the animation doesn't do more harm than good.
          </p>
          <p>
            Sometimes, the sole purpose of an animation could be to bring delight and that is perfectly valid, especially if the
            goal was always to create a delightful experience.
          </p>
          <b> A 'practical' example is the draggable pills on The Content Nerd. Delightful! </b>
          <video src="https://cdn.whatwouldgoodydo.com/video-tsd75s.webm" muted loop playsinline />
        </div>

        <h2 id="Storytelling">8 .{{ "  " }}Storytelling</h2>
        <div>
          <p>
            The primary purpose of a website has always been to facilitate the sharing, access, and exchange of information
            globally and we can achieve that easier through stories.
          </p>
          <p>
            We can use real-time data for dynamic storytelling, allowing users to manipulate variables and see immediate changes.
            Scrollytelling is another effective form of storytelling on the web, where the scroll reveals the narrative gradually
            while keeping the user in control.
          </p>
          <p>
            Interactive experiences generally turn the user into a character in the story, making the journey engaging, memorable,
            and conducive to virtually any goal.
          </p>
          <b>
            A practical example is the PVSR '24 which focuses on storytelling and letting users play with data and visualize
            insights.
          </b>
          <video src="https://cdn.whatwouldgoodydo.com/video-yf5wsu.webm" muted loop playsinline />
        </div>

        <h2 id="Feedback">9 .{{ "  " }}Feedback</h2>
        <div>
          <p>
            Animations should be fast, especially for frequently used elements. Although perceived speed varies based on the
            easing and size of element, a duration between 100ms and 300ms is usually the sweet spot
          </p>
          <p>
            When an action is triggered by human interaction, the websites must provide immediate feedback. To make our website
            feel more responsive, we should significantly reduce the duration of animations, avoid easing them in or even remove
            animations entirely to prevent user fatigue if need be.
          </p>
          <p>
            Websites should also subtly "hint" at the outcome of interactions. This makes actions feel expected and predictable.
            Feedback helps to drive the user's attention to the relevant part of our website and confirms their status within the
            experience. It should answer all their questions regarding "Where, When, and How."
          </p>
          <b> A practical example is the snappy experience of the visitors page in AJ's portfolio. </b>
          <video src="https://cdn.whatwouldgoodydo.com/video-jsnj21s.webm" muted loop playsinline />
        </div>

        <h2 id="Life">10 .{{ "  " }}Life</h2>
        <div>
          <p>
            To bring our websites to life, our elements and animations should possess the qualities of living matter, being able
            'metabolize', 'reproduce', grow, and respond to environmental stimuli.
          </p>
          <p>
            We should infer relationships between elements and events without requiring direct human input. This involves using
            secondary information and actions, magnetic fields, self-triggered animations, and adaptive cursors.
          </p>
          <p>
            Our website should be resilient, it should have the ability to reset after disruptions, acknowledge causation and
            provide users with rewards (or consequences) as they interact with it
          </p>
          <b>
            A practical example is the secondary cursor in Library. It moves autonomously and follows you as you scroll, behaving
            just like a living assistant.
          </b>
          <video src="https://cdn.whatwouldgoodydo.com/video-su82so.webm" muted loop playsinline />
        </div>

        <h2 id="Language">11 .{{ "  " }}Language</h2>
        <div>
          <p>
            No website is ever standalone. It is an extension of a product, service, brand, or even its creators. Therefore, we
            must leverage motion design languages, principles, and guidelines to ensure consistency and maintain a sense of
            continuity.
          </p>
          <p>
            We must make conscious decisions about how and when elements move. Without a distinct motion language, websites feel
            generic and lose their memorability.
          </p>
          <p>
            To enforce brand personality, we can aslo add animations solely for decoration. These serve to subconsciously embed
            the brand's essence into the user's mind.
          </p>
          <b>A pratical example is the looping hero images in Onchain Dreamers which enforces Onboard's brand and personality</b>
          <video src="https://cdn.whatwouldgoodydo.com/video-hww8s2.webm" muted loop playsinline />
        </div>

        <h2 id="Mimick">12 .{{ "  " }}Mimick</h2>
        <div>
          <p>
            Beyond simple kinematics, we should apply the laws of physics to our animations, like weight, inertia, bounce,
            elasticity and friction. The goal is to mimick and simulate how objects move and react in the real world so accurately
            that the animation feels fluid and "real".
          </p>
          <p>
            Beyond physics, there is also room to explore Augmented Reality, overlaying digital information onto the real world
            environment, we could visualize our websites as if they were actually in front of us, utilizing virtual interactions,
            spatial sound, and voice commands.
          </p>
          <p>
            We are limited only by current technology, but that barrier grows thinner every day. AR makes complex concepts
            tangible, reducing cognitive load to near zero and shooting accessibility through the roof. We can already integrate
            some concepts with concepts like allowing users to interact with 3D elements, and adding sound design to our
            experiences.
          </p>
          <b>
            A practical example is the Booking experience of the Garage. Uses 3d to visulaize and interact with the actual space
          </b>
          <video src="https://cdn.whatwouldgoodydo.com/video-rt58ig.webm" muted loop playsinline />
        </div>

        <div>
          <br />
          <p>
            Web Animation could serve as the bridge between websites and the human mind. It is the difference between a user
            simply viewing content and truly experiencing it.
          </p>
          <p>
            These principles are not rigid laws, not even for me, and we certainly don't have to use them all together. The core
            mission remains to create delightful experiences. and when used with purpose and grace, we stop building mere websites
            and start building web portals and worlds
          </p>
          <br />
          <br />
        </div>
      </div>
    </div>
  </main>
</template>

<script setup lang="ts">
const projName = ref(`12 Principles of Animation`);
const projDesc = ref(
  `Web Animation could serve as the bridge between websites and the human mind. It is the difference between a user simply viewing content and truly experiencing it.`,
);
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
  const videos = document.querySelectorAll<HTMLVideoElement>(".article-body video");

  const observer = new IntersectionObserver(
    (entries) => {
      entries.forEach((entry) => {
        const video = entry.target as HTMLVideoElement;
        if (entry.isIntersecting) {
          video.play();
        } else {
          video.pause();
          video.currentTime = 0;
        }
      });
    },
    { threshold: 0.3 },
  );

  videos.forEach((video) => observer.observe(video));

  onBeforeUnmount(() => observer.disconnect());
});
</script>
