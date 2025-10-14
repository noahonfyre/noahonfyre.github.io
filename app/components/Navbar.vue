<template>
  <nav class="grid grid-flow-col py-6">
    <div class="flex items-center h-full">
      <NuxtLink to="/">
        <svg viewBox="0 0 18 8" fill="none" xmlns="http://www.w3.org/2000/svg" class="h-8">
        <path fill-rule="evenodd" clip-rule="evenodd" d="M0.5 8L8.5 0L8.5 8H6.5V4.5L3 8H0.5Z" fill="currentColor"/>
        <path fill-rule="evenodd" clip-rule="evenodd" d="M17.5 0L9.5 8L9.5 -6.99382e-07L11.5 -5.24537e-07L11.5 3.5L15 -2.18557e-07L17.5 0Z" fill="currentColor"/>
      </svg>
      </NuxtLink>
    </div>

    <div class="flex justify-end items-center">
      <NuxtLink class="font-display font-bold py-2 px-6 hover:text-element-950 ease-in-out duration-150" v-for="item in navItems" :to="item.to">{{ item.text }}</NuxtLink>
    </div>
  </nav>
</template>

<script setup>
const navItems = [
  { text: "Introduction", to: "/" },
  { text: "Technologies", to: "/" },
  { text: "Projects", to: "/" },
  { text: "Experience", to: "/" },
  { text: "About", to: "/" },
]
</script>