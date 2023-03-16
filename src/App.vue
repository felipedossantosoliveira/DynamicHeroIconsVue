<script setup>
import RenderIcon from "./components/RenderIcon.vue";

const icons = ["CubeIcon", "BeakerIcon", "BugAntIcon", "GlobeAmericasIcon"];
</script>

<template>
  <div class="bg-slate-100 h-[720px]">
    <header class="p-10 w-full flex flex-col">
      <h1 class="font-bold text-xl text-center">Dynamic Load Icons</h1>
      <h2 class="font-semibold underline text-lg text-center">
        <a href="https://heroicons.com/"> Heroicons Library </a>
      </h2>
    </header>
    <div class="px-10">
      <RenderIcon />
    </div>
  </div>
</template>