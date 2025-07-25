<template>
  <div class="grid grid-cols-2">
    <img
      src="../assets/food1.jpg"
      class="w-full h-100 object-cover border-solid border-4 border-collapse border-bordeaux"
    />
    <img
      src="../assets/food2.jpg"
      class="w-full h-100 object-cover border-solid border-4 border-collapse border-bordeaux"
    />
  </div>

  <div
    class="bg-bordeaux w-full grid lg:grid-cols-2 sm:grid-cols-1 py-3 px-2 gap-2 lg:divide-white"
  >
    <div class="contact-div px-5">
      <p class="font-homemadeapple text-white text-2xl py-1.5">Contact us!</p>
      <div class="text-inter text-white px-2">
        <p class="py-1">Phone Number: +1 (506) 408-0025</p>
        <p class="py-1">Email Address: lysa@noblebythesea.com</p>
        <p class="py-1">Civic Address: 132 Water St., Saint Andrews, NB</p>
      </div>
    </div>

    <div class="hours-div px-1.5">
      <p class="font-homemadeapple text-white text-2xl py-1.5">Noble Hours</p>
      <div class="text-inter text-white px-2">
        <p class="py-1">Closed on Mondays</p>
        <p class="py-1">Tuesday to Saturday 12:00pm - 11:00pm</p>
        <p class="py-1">Sunday 12:00pm - 10:00pm</p>
      </div>
    </div>
  </div>
</template>

<script setup></script>
