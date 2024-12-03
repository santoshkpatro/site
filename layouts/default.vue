<script setup></script>

<template>
  <div class="min-h-screen border-8 border-purple-500 py-6 px-12 flex flex-col">
    <!-- Navbar -->
    <header class="flex justify-between items-center mb-6">
      <h1 class="text-xl font-bold text-purple-500">Santosh Kumar Patro</h1>
      <nav>
        <ul class="flex space-x-6 text-lg">
          <li>
            <NuxtLink to="/" class="text-gray-700 hover:text-purple-500"
              >Home</NuxtLink
            >
          </li>
          <li>
            <NuxtLink to="/blogs" class="text-gray-700 hover:text-purple-500"
              >Blogs</NuxtLink
            >
          </li>
          <li>
            <NuxtLink
              to="https://github.com/santoshkpatro"
              class="text-gray-700 hover:text-purple-500 font-semibold"
              target="_blank"
              rel="noopener noreferrer"
            >
              GitHub
            </NuxtLink>
          </li>
          <li>
            <NuxtLink
              to="https://x.com/santoshkpatro_"
              class="text-gray-700 hover:text-purple-500 font-semibold"
              target="_blank"
              rel="noopener noreferrer"
            >
              X
            </NuxtLink>
          </li>
        </ul>
      </nav>
    </header>

    <!-- Main Content -->
    <main class="flex-grow">
      <slot />
    </main>

    <!-- Footer -->
    <footer class="mt-2 text-center text-gray-600">
      <p>© 2024 Santosh Kumar Patro. All rights reserved.</p>
    </footer>
  </div>
</template>
