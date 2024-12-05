<script setup>
const currentPage = ref(1);
const pageSize = 3;
const articles = await queryContent("blogs")
  .sort({ date: -1 })
  .skip((currentPage.value - 1) * pageSize)
  .limit(pageSize)
  .find();
const totalArticles = await queryContent('blogs').count()
const totalPages = Math.ceil(totalArticles / pageSize);

import dayjs from "dayjs";
useHead({
  title: `Blogs | Santosh Kumar Patro`
})
</script>

<template>
  <div class="max-w-4xl mx-auto p-4">
    <!-- Blog Header -->
    <header class="mb-6">
      <h1 class="text-5xl font-bold text-black">
        Blogs<span class="text-purple-500">.</span>
      </h1>
    </header>

    <!-- Blog Articles -->
    <div class="space-y-6">
      <div v-for="article in articles" :key="article.title">
        <!-- Date -->
        <p class="text-sm font-medium text-gray-500 mb-1">
          {{ dayjs(article.date).format("MMM D, YYYY") }}
        </p>
        <!-- Title -->
        <h2
          class="text-3xl font-extrabold text-purple-600 mb-1 hover:underline hover:underline-offset-2 cursor-pointer"
        >
          <NuxtLink :to="article._path">
            {{ article.title }}
          </NuxtLink>
        </h2>
        <!-- Description -->
        <p class="text-gray-700 leading-relaxed">
          {{ article.description }}
        </p>
      </div>
    </div>

    <!-- Pagination -->
    <div class="mt-8 flex">
      <button
        class="px-2 py-1 bg-purple-500 text-white rounded-l-md hover:bg-purple-600"
        :disabled="currentPage === 1"
        @click="currentPage--"
      >
        <<
      </button>
      <span class="px-2 py-1 bg-purple-500 text-white">
        {{ currentPage }}
      </span>
      <button
        class="px-2 py-1 bg-purple-500 text-white rounded-r-md hover:bg-purple-600"
        :disabled="currentPage === totalPages"
        @click="currentPage++"
      >
        >>
      </button>
    </div>
  </div>
</template>
