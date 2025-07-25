<template>
  <section>
    <div class="herosection w-full h-100 bg-[url(/src/assets/hero.jpg)]">
      <nav>
        <router-link to="/">
          <img
            class="absolute w-36 h-auto ml-2"
            src="/src/assets/NobleLogo.png"
          />
        </router-link>
        <ul class="hidden md:flex justify-center pt-8 gap-x-4 font-inter">
          <li class="nav-link">
            <router-link to="/" class="text-white hover:bg-bordeaux p-2 rounded"
              >Home</router-link
            >
          </li>
          <li class="nav-link">
            <router-link
              to="/about"
              class="text-white hover:bg-bordeaux p-2 rounded"
              >About</router-link
            >
          </li>
          <li class="nav-link">
            <router-link
              to="/menu"
              class="text-white bg-gray-200/45 hover:bg-bordeaux p-2 rounded"
              >Menu</router-link
            >
          </li>
        </ul>
      </nav>
    </div>
    <div class="textsection bg-bordeaux">
      <h1 class="text-3xl md:text-6xl font-kingred py-2 px-15 text-driftwood">
        NOBLE Menu
      </h1>
      <p class="font-inter text-driftwood py-5 px-15">
        At NOBLE, we believe that the freshest flavors come straight from our
        community. That’s why we proudly partner with local farmers, growers,
        and artisans to bring you ingredients at their seasonal peak. Our menu
        is a vibrant reflection of what’s fresh and abundant, changing regularly
        to celebrate the rhythms of the harvest. Whether it’s heirloom tomatoes
        in the summer or root vegetables in the fall, every dish is crafted to
        highlight nature’s best. Every visit brings something new and delicious
        to discover.
      </p>
    </div>
  </section>
</template>

<script setup></script>
