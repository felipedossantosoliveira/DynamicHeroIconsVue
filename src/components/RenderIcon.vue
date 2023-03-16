<script setup>
import * as heroicon from "@heroicons/vue/24/outline";
import ProcessingIcon from "./ProcessingIcon.vue";
import { reactive } from "vue";

const icon = reactive({
  data: "BugAntIcon",
});
</script>
<template>
  <div class="flex space-x-4 items-end">
    <div class="flex-1">
      <label for="icon" class="font-semibold">Icon name:</label>
      <input
        type="text"
        v-model="icon.data"
        class="block p-4 w-full rounded-md border-2 bg-violet-50 border-violet-300 shadow-lg focus:border-sky-500 focus:ring-sky-500"
      />
    </div>
    <div class="flex flex-none items-center justify-center">
      <div class="p-3 bg-violet-50 border-2 rounded-md border-violet-300">
        <component
          :is="heroicon[icon.data] ? heroicon[icon.data] : ProcessingIcon"
          class="w-8"
        />
      </div>
    </div>
  </div>
</template>