<template>
  <div class="w-full border-b flex items-center justify-center bg-transparent z-50">
    <div
      class="flex items-center justify-between px-4 text-black d md:px-8 py-2"
    >
      <div class="flex items-center">
        <nuxt-link to="/">
          <nuxt-img
            src="/icologo.png"
            alt="Logo"
            format="webp"
            class="h-6 sm:h-12 md:h-18 pr-4"
            sizes="sm:100vw md:100vw lg:400px"
          />
        </nuxt-link>
      </div>
      <button
        @click="toggleMenu()"
        class="md:hidden p-2 rounded focus:outline-none focus:ring-2 focus:ring-gray-400"
      >
        <Icon
          :name="isMenuOpen ? 'pajamas:close' : 'pajamas:hamburger'"
          class="w-6 h-6 text-gray-700"
        />
      </button>
      <!-- Desktop menu -->
      <ul
        class="hidden md:flex text-sm sm:text-lg md:text-2xl flex-row text-black text-shadow navbar font-mono"
      >
        <li class="hover:scale-110">
          <nuxt-link to="/" class="pl-4 sm:pl-8 md:pl-12 lg:pl-16"
            >Home</nuxt-link
          >
        </li>
        <li class="hover:scale-110">
          <nuxt-link to="/about" class="pl-4 sm:pl-8 md:pl-12 lg:pl-16"
            >About</nuxt-link
          >
        </li>
        <li class="hover:scale-110">
          <nuxt-link to="/services" class="pl-4 sm:pl-8 md:pl-12 lg:pl-16"
            >Services</nuxt-link
          >
        </li>

        <li class="hover:scale-110">
          <nuxt-link to="/contact" class="pl-4 sm:pl-8 md:pl-12 lg:pl-16"
            >Contact</nuxt-link
          >
        </li>
      </ul>
    </div>
    <ul
      v-if="isMenuOpen"
      class="block md:hidden mt-56 absolute z-10 m-auto left-0 w-2/4 right-0 bg-transparent border rounded-lg text-center font-mono"
    >
      <li>
        <nuxt-link
          to="/"
          class="block py-2 px-4 text-black pl-8 hover:text-gray-900 hover:scale-110"
          aria-current="page"
          >Home</nuxt-link
        >
      </li>
      <li>
        <nuxt-link
          to="/about"
          class="block py-2 px-4 text-black pl-8 hover:text-gray-900 hover:scale-110"
          >Portfolio</nuxt-link
        >
      </li>
      <li>
        <nuxt-link
          to="/services"
          class="block py-2 px-4 text-black pl-8 hover:text-gray-900 hover:scale-110"
          aria-current="page"
          >About</nuxt-link
        >
      </li>
      <li>
        <nuxt-link
          to="/contact"
          class="block py-2 px-4 text-black pl-8 hover:text-gray-900 hover:scale-110"
          >Contact</nuxt-link
        >
      </li>
    </ul>
  </div>
</template>
<script setup>
const isMenuOpen = ref(false);

const toggleMenu = () => {
  isMenuOpen.value = !isMenuOpen.value;
};
// Add event listener to close the menu when clicking outside
</script>
