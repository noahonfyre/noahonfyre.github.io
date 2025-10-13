<template>
  <section class="h-full grid grid-cols-3 grid-rows-3 gap-3">
    <div class="flex flex-col bg-element-50 text-element-950 rounded-2xl col-span-1 row-span-1"></div>
    <div class="bg-element-50 text-element-950 p-3 rounded-2xl col-span-2 row-span-2">test</div>
    <div class="bg-element-50 text-element-950 p-3 rounded-2xl col-span-1 row-span-2">test</div>
    <div class="bg-element-50 text-element-950 px-6 py-12 rounded-2xl col-span-2 row-span-1">
      <div class="grid place-items-center w-full h-full">
        <div class="bg-element-100 rounded-xl grid grid-flow-col place-items-center divide-x-2 divide-element-50 w-full h-full">
          <div class="flex flex-col justify-center items-center w-full h-full" v-for="item in stats">
            <h1 class="font-bold text-4xl">{{ item.title }}</h1>
            <p>{{ item.description }}</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup lang="ts">
const { data } = await useFetch("https://api.github.com/users/noahonfyre")

const stats = ref([
  { title: "1700", description: "Total Commits" },
  { title: "60", description: "Resolved Pull Requests" },
  { title: "25", description: "Stars on Repositories" },
  { title: "4+", description: "Projects completed" },
])
</script>