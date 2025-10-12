<template>
  <div class="w-screen h-screen">
    <div class="relative w-full h-3/4 bg-frankfurt bg-cover bg-no-repeat bg-top">
      <div class="absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 z-0">
        <div class="flex items-center justify-between">
          <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" class="size-10 text-element-950">
            <path stroke-linecap="round" stroke-linejoin="round" d="M15 10.5a3 3 0 1 1-6 0 3 3 0 0 1 6 0Z" />
            <path stroke-linecap="round" stroke-linejoin="round" d="M19.5 10.5c0 7.142-7.5 11.25-7.5 11.25S4.5 17.642 4.5 10.5a7.5 7.5 0 1 1 15 0Z" />
          </svg>
          <h1 class="font-display font-bold text-element-950 text-4xl tracking-tighter">HESSEN, GERMANY</h1>
        </div>
        <h1 class="font-display font-black text-element-950 text-9xl tracking-tighter">FRANKFURT</h1>
      </div>
      <div class="absolute top-0 left-0 w-full h-full bg-frankfurt-fg bg-cover bg-no-repeat bg-top z-10"></div>
    </div>
  </div>
</template>

<style scoped>
.bg-frankfurt {
  background-image: url("/img/frankfurt_full.png");
}
.bg-frankfurt-fg {
  background-image: url("/img/frankfurt_fg.png");
}
</style>
<script setup lang="ts">
</script>