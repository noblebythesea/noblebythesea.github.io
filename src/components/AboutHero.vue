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
              class="text-white bg-gray-200/45 hover:bg-bordeaux p-2 rounded"
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
    <div class="textsection bg-bordeaux">
      <h1 class="text-3xl md:text-6xl font-kingred py-2 px-15 text-driftwood">
        About NOBLE
      </h1>
      <p class="font-inter text-driftwood py-5 px-15">
        Nestled within the historic Windsor House in the charming seaside town
        of St. Andrews, New Brunswick, NOBLE offers a one-of-a-kind dining
        experience where heritage meets contemporary cuisine. Our ever-evolving,
        locally inspired menu celebrates the best of the region’s seasonal
        ingredients, paired with artisan cocktails and a carefully curated list
        of regional craft beers. Whether you're joining us for a cozy dine-in
        experience, enjoying the fresh air in our beautiful courtyard, or
        picking up a thoughtfully prepared takeout meal, NOBLE brings warmth,
        flavor, and hospitality to every moment. We also welcome reservations
        and offer full catering services, making us the perfect choice for your
        next event or special occasion. With a fully stocked bar and a passion
        for culinary excellence, NOBLE invites you to savor the taste of New
        Brunswick one plate at a time.
      </p>
    </div>
  </section>
</template>

<script setup></script>
