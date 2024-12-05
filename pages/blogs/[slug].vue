<script setup>
const route = useRoute()

const article = await queryContent("blogs").where({ _path: route.path }).findOne()
await useSeoMeta({
  title: article.title,
  ogTitle: article.title,
  description: article.description,
  ogDescription: article.description
})
await useHead({
  title: `${article.title} | Santosh Kumar Patro`
})
</script>

<template>
  <ContentDoc v-slot="{ doc }">
    <div class="flex flex-col">
        <div class="mb-6 mt-2">
            <h1 class="text-5xl font-extrabold">{{ doc.title }}</h1>
        </div>

        <div>
            <ContentRenderer :value="doc" />
        </div>
    </div>
  </ContentDoc>
</template>
