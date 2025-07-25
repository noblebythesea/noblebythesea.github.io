<template>
  <div class="md:hidden fixed top-[60px] right-0 w-full z-50">
    <div class="flex p-4 text-white">
      <button @click="toggleMenu" class="focus:outline-none">
        <svg
          class="w-6 h-6"
          fill="none"
          stroke="currentColor"
          stroke-width="2"
          viewBox="0 0 24 24"
          stroke-linecap="round"
          stroke-linejoin="round"
        >
          <path d="M4 6h16M4 12h16M4 18h16" />
        </svg>
      </button>
    </div>

    <div v-if="menuOpen" class="bg-bordeaux/50 text-white">
      <router-link to="/" class="block px-4 py-2 hover:bg-noblenavy"
        >Home</router-link
      >
      <router-link to="/about" class="block px-4 py-2 hover:bg-noblenavy"
        >About</router-link
      >
      <router-link to="/menu" class="block px-4 py-2 hover:bg-noblenavy"
        >Menu</router-link
      >
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";
const menuOpen = ref(false);
const toggleMenu = () => {
  menuOpen.value = !menuOpen.value;
};
</script>
