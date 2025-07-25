<script setup>
import Banner from "@/components/Banner.vue";
import Footer from "./components/Footer.vue";
import SidebarMenu from "./components/SidebarMenu.vue";
</script>

<template>
  <Banner
    :announcements="[
      'Happy hour starts at 3:00pm everyday! Enjoy discounted cocktails and draft beer!',
      'Check our social media for live music updates!',
      'Menu offerings can change each day. Come and see if we have your favourite, or try something new!',
    ]"
  />
  <SidebarMenu />
  <RouterView />
  <Footer />
</template>

<style scoped></style>
