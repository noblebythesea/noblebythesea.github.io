<template>
  <footer class="bg-harbourhaze text-white mt-10 py-10">
    <div class="max-w-6xl mx-auto px-4 grid grid-cols-1 md:grid-cols-3 gap-8">
      <div>
        <img src="/src/assets/NobleCCWhite.png" alt="Noble Logo" class="w-60" />
        <p>132 Water Street, St. Andrews, NB</p>
        <p>Hours: 10:00am to 10:00pm Mon–Sun</p>
        <p>Phone: (506) 408-0025</p>
        <div class="flex space-x-4 mt-4">
          <a href="#"
            ><img src="/src/assets/instagram.svg" alt="Instagram" class="w-10"
          /></a>
          <a href="#"
            ><img src="/src/assets/facebook.svg" alt="Facebook" class="w-10"
          /></a>
        </div>
      </div>
      <div class="pt-10">
        <h4 class="font-bold mb-2">Explore</h4>
        <ul>
          <li>
            <router-link to="/about" class="hover:underline">About</router-link>
          </li>
          <li>
            <router-link to="/menu" class="hover:underline">Menu</router-link>
          </li>
        </ul>
      </div>
      <div class="pt-10">
        <h4 class="font-bold mb-2">Resources</h4>
        <ul>
          <li><a href="#" class="hover:underline">Blog</a></li>
        </ul>
      </div>
    </div>
  </footer>
</template>

<script setup></script>
