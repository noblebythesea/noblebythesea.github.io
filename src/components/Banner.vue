<script setup>
import { ref, computed, onMounted, onBeforeUnmount } from "vue";

const props = defineProps({
  announcements: {
    type: Array,
    required: true,
  },
});

const currentIndex = ref(0);
const fading = ref(false);
let intervalId = null;

const currentAnnouncement = computed(
  () => props.announcements[currentIndex.value]
);

function nextAnnouncement() {
  fading.value = true;
  setTimeout(() => {
    currentIndex.value = (currentIndex.value + 1) % props.announcements.length;
    fading.value = false;
  }, 300);
}

function previousAnnouncement() {
  fading.value = true;
  setTimeout(() => {
    currentIndex.value =
      (currentIndex.value - 1 + props.announcements.length) %
      props.announcements.length;
    fading.value = false;
  }, 300);
}

function startRotation() {
  intervalId = setInterval(nextAnnouncement, 6000);
}

function stopRotation() {
  clearInterval(intervalId);
}

onMounted(startRotation);
onBeforeUnmount(stopRotation);
</script>

<template>
  <div
    id="banner"
    class="flex items-center justify-center bg-noblenavy text-white py-3 px-4"
    @mouseenter="stopRotation"
    @mouseleave="startRotation"
  >
    <button
      @click="previousAnnouncement"
      class="absolute px-2 py-1 text-white text-3xl rounded hover:bg-gray-200/25 left-0"
    >
      ‹
    </button>
    <transition name="fade">
      <span :key="currentAnnouncement" class="text-md font-kingred">{{
        currentAnnouncement
      }}</span>
    </transition>
    <button
      @click="nextAnnouncement"
      class="absolute px-2 py-1 text-white text-3xl rounded hover:bg-gray-200/25 right-0"
    >
      ›
    </button>
  </div>
</template>

<style scoped>
.bg-navy {
  background-color: #111c4e;
}

.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.3s ease;
}
.fade-enter-from,
.fade-leave-to {
  opacity: 0;
}
</style>
