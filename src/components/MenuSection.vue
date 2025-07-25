<template>
  <section class="p-6 max-w-4xl mx-auto">
    <h1 class="text-2xl font-homemadeapple mb-4 text-center">Our Menus</h1>

    <div class="mb-6 text-center">
      <label for="menuSelect" class="mr-2 font-medium">Choose a menu:</label>
      <select
        id="menuSelect"
        v-model="selectedMenu"
        class="border px-3 py-2 rounded text-black"
      >
        <option value="NOBLELunchMenu">Lunch</option>
        <option value="NOBLEDinnerMenu">Dinner</option>
      </select>
    </div>

    <div class="relative w-full h-[600px] border shadow-md">
      <iframe
        :src="pdfSrc"
        class="w-full h-full"
        frameborder="0"
        title="Menu PDF"
      ></iframe>
    </div>
  </section>
</template>

<script setup>
import { ref, computed } from "vue";

const selectedMenu = ref("NOBLELunchMenu");

const pdfSrc = computed(() => {
  return `/menus/${selectedMenu.value}.pdf`;
});
</script>
