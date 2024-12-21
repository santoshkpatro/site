<script setup>
useSeoMeta({
  title: "Santosh Kumar Patro",
  ogTitle: "Santosh Kumar Patro",
  description:
    "I’m a polyglot developer who’s equally comfortable wrangling Django, Vue.js, Ruby on Rails, and Go. Think of me as a Swiss Army knife of coding—effective and occasionally sarcastic",
  ogDescription:
    "I’m a polyglot developer who’s equally comfortable wrangling Django, Vue.js, Ruby on Rails, and Go. Think of me as a Swiss Army knife of coding—effective and occasionally sarcastic",
});

useHead({
  title: "Santosh Kumar Patro",
});
</script>

<template>
  <main class="flex flex-col p-6">
    <div class="max-w-4xl mx-auto">
      <!-- Big Heading -->
      <h1 class="text-5xl font-bold text-gray-800 mb-4">
        Hi there! <span class="wave">👋</span>
      </h1>

      <!-- Current Position -->
      <p class="text-2xl text-gray-700 mb-2">
        I'm a
        <span class="font-semibold text-gray-900 jazz"
          >Senior <span class="line-through">Full</span> Any Stack
          Engineer</span
        >
        at
        <span
          class="font-semibold text-blue-600 jazz cursor-pointer italic underline"
        >
          <NuxtLink to="https://acornglobus.com" target="_blank"
            >AcornGlobus</NuxtLink
          > </span
        >, where I craft everything from
        <span class="font-semibold text-gray-800 jazz">robust backends</span> to
        <span class="font-semibold text-gray-800 jazz">jazzy frontends</span>.
      </p>

      <!-- About Me -->
      <p class="text-2xl text-gray-700 leading-relaxed">
        I'm a polyglot developer who's equally comfortable wrangling
        <span class="font-semibold text-gray-800 jazz">Django</span>,
        <span class="font-semibold text-gray-800 jazz">Vue.js</span>,
        <span class="font-semibold text-gray-800 jazz">Ruby on Rails</span>, and
        <span class="font-semibold text-gray-800 jazz">Go</span>. Think of me as
        a tech polymath—effective and occasionally sarcastic.
      </p>

      <p class="text-2xl text-gray-700 leading-relaxed mt-2">
        I've also built <span class="font-semibold jazz">Shopify apps</span> and
        am actively working on my passion project:
      </p>

      <div class="mt-4">
        <h2 class="text-3xl font-bold text-gray-800 mb-2">🚀 Calyvim</h2>
        <p class="text-2xl text-gray-700 leading-relaxed">
          <span
            class="text-blue-600 font-semibold jazz cursor-pointer underline italic"
          >
            <NuxtLink to="https://calyvim.com" target="_blank"
              >Calyvim</NuxtLink
            >
          </span>
          is an open-source project/product management tool to streamline
          business workflows.
        </p>
      </div>

      <div class="mt-6">
        <h2 class="text-3xl font-bold text-gray-800 mb-2">
          🏸 Off the Keyboard
        </h2>
        <p class="text-2xl text-gray-700 leading-relaxed">
          When I'm not coding, you can find me smashing shuttlecocks on the
          badminton court.
        </p>
      </div>

      <!-- Contact -->
      <p class="text-2xl text-gray-700 leading-relaxed mt-2">
        Want to read more about my thoughts and ideas?
        <NuxtLink
          to="/blogs"
          target="_blank"
          class="text-blue-600 underline font-semibold jazz italic"
        >
          Click here to check out my blogs!
        </NuxtLink>
      </p>

      <p class="text-2xl text-gray-700 leading-relaxed mt-2">
        Feel free to reach out on
        <span class="font-bold italic jazz text-blue-600 underline">
          <NuxtLink to="https://x.com/santoshkpatro_" target="_blank"
            >X</NuxtLink
          >
        </span>
        or email me at
        <a
          href="mailto:santoshkpatro11@gmail.com"
          class="text-blue-600 underline jazz italic"
        >
          hey@santoshkpatro.in </a
        >.
      </p>

      <!-- Caption -->
      <p class="text-xl text-gray-900 font-bold mt-4">
        "Coding through caffeine, smashing birdies, and chasing big dreams with
        passion."
      </p>
    </div>
  </main>
</template>

<style>
.wave {
  animation: wave-animation 1.5s infinite;
  display: inline-block;
}

@keyframes wave-animation {
  0%,
  60%,
  100% {
    transform: rotate(0deg);
  }

  30% {
    transform: rotate(-10deg);
  }
}

/* Hover effect for bold text */
.jazz:hover {
  background-color: #8b5cf6;
  /* Primary color */
  color: white;
  /* Text color becomes white */
}
</style>
