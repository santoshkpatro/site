<script setup>
useSeoMeta({
  title: "Santosh Kumar Patro",
  ogTitle: "Santosh Kumar Patro",
  description:
    "I’m a polyglot developer who’s equally comfortable wrangling Django, Vue.js, Ruby on Rails, and Go. Think of me as a Swiss Army knife of coding—effective and occasionally sarcastic",
  ogDescription:
    "I’m a polyglot developer who’s equally comfortable wrangling Django, Vue.js, Ruby on Rails, and Go. Think of me as a Swiss Army knife of coding—effective and occasionally sarcastic",
});
</script>

<template>
  <main class="flex flex-col justify-center items-center text-center p-6">
    <div class="max-w-4xl">
      <!-- Big Heading -->
      <h1 class="text-5xl font-bold text-gray-800 mb-4">
        Hi there! <span class="wave">👋</span>
      </h1>

      <!-- Current Position -->
      <p class="text-2xl text-gray-700 mb-2">
        I’m a
        <span class="font-semibold text-gray-900 jazz"
          >Senior <span class="line-through">Full</span> Any Stack
          Engineer</span
        >
        at
        <span class="font-semibold text-blue-600 jazz cursor-pointer italic underline">
          <NuxtLink to="https://acornglobus.com" target="_blank"
            >AcornGlobus</NuxtLink
          > </span
        >, where I craft everything from
        <span class="font-semibold text-gray-800 jazz">robust backends</span> to
        <span class="font-semibold text-gray-800 jazz">jazzy frontends</span>.
      </p>

      <!-- About Me -->
      <p class="text-2xl text-gray-700 leading-relaxed">
        I’m a polyglot developer who’s equally comfortable wrangling
        <span class="font-semibold text-gray-800 jazz">Django</span>,
        <span class="font-semibold text-gray-800 jazz">Vue.js</span>,
        <span class="font-semibold text-gray-800 jazz">Ruby on Rails</span>, and
        <span class="font-semibold text-gray-800 jazz">Go</span>. Think of me as
        a Swiss Army knife of coding—effective and occasionally sarcastic.
      </p>

      <p class="text-2xl text-gray-700 leading-relaxed mt-2">
        I’ve also built <span class="font-semibold jazz">Shopify apps</span>,
        smashed birdies on the
        <span class="font-semibold jazz">badminton court 🏸</span>, and am
        actively working on two side projects:
      </p>

      <div class="mt-2">
        <ul class="list-none">
          <li class="text-2xl text-blue-600 font-semibold">
            <span class="jazz cursor-pointer underline italic">
              <NuxtLink
                to="https://github.com/santoshkpatro/taskite"
                target="_blank"
                >Taskite</NuxtLink
              > </span
            >:
            <span class="text-gray-700"
              >An open-source project management tool.</span
            >
          </li>
          <li class="text-2xl text-blue-600 font-semibold mt-2">
            <span class="jazz cursor-pointer underline italic">
              <NuxtLink
                to="https://github.com/santoshkpatro/calyvim"
                target="_blank"
                >Calyvim</NuxtLink
              > </span
            >:
            <span class="text-gray-700"
              >An invoicing and book-keeping tool.</span
            >
          </li>
        </ul>
      </div>

      <!-- Contact -->
      <p class="text-2xl text-gray-700 leading-relaxed mt-2">
        Want to read more about my thoughts and ideas?
        <NuxtLink to="/blogs" target="_blank" class="text-blue-600 underline font-semibold jazz italic">
          Click here to check out my blogs!
        </NuxtLink>
      </p>

      <p class="text-2xl text-gray-700 leading-relaxed mt-2">
        Feel free to reach out on
        <span class="font-bold italic jazz"
          ><NuxtLink to="https://x.com/santoshkpatro_" target="_blank"
            >X</NuxtLink
          ></span
        >
        or email me at
        <a
          href="mailto:santoshkpatro11@gmail.com"
          class="text-blue-600 underline jazz italic"
        >
          hey@santoshkpatro.in</a
        >.
      </p>

      <!-- Caption -->
      <p class="text-3xl text-gray-900 font-bold mt-4">
        "Coding through caffeine, smashing birdies, and chasing big dreams—one
        commit at a time."
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
