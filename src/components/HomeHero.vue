<template>
  <section>
    <div class="herosection w-full h-100 bg-[url(/src/assets/hero.jpg)]">
      <nav>
        <a href="#">
          <img
            class="absolute w-36 h-auto ml-2"
            src="/src/assets/NobleLogo.png"
        /></a>
        <ul class="hidden md:flex justify-center pt-8 gap-x-4 font-inter">
          <li class="nav-link">
            <router-link
              to="/"
              class="text-white bg-gray-200/45 hover:bg-bordeaux p-2 rounded"
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
              class="text-white hover:bg-bordeaux p-2 rounded"
              >Menu</router-link
            >
          </li>
        </ul>
      </nav>
    </div>
    <div class="textsection">
      <h1
        class="text-3xl md:text-4xl font-kingred text-center py-2 text-noblenavy"
      >
        EAT, DRINK & BE MERRY
      </h1>
      <p class="font-inter py-7 px-30 text-center">
        NOBLE, located in the picturesque town of St. Andrews, New Brunswick,
        Canada, is a distinctive culinary destination offering heritage-inspired
        dining experiences. Catering to both discerning food enthusiasts and
        tourists, the restaurant provides an inviting open-air dining experience
        complemented by artisan cocktails and a curated selection of regional
        craft beers.
      </p>
      <p class="font-inter text-center">
        <router-link to="/about" class="text-noblenavy hover:underline"
          >Learn More</router-link
        >
      </p>
    </div>
  </section>
</template>

<script setup></script>
