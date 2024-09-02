<template>
  <div>

  <nav class="bg-transparent text-white py-4 fixed w-full top-0 z-40 font-index text-2xl">
    <div class="container mx-auto flex items-center justify-between px-6">
      <a href="#home" class="text-3xl font-bold "></a>
      <ul class="flex space-x-6">
        <li>
          <a href="#home" class="hover:text-red-600 transition">Home</a>
        </li>
        <li>
          <a href="#second-page" class="hover:text-red-600 transition">The Darkness</a>
        </li>
        <li>
          <a href="#contact" class="hover:text-red-600 transition">Contact</a>
        </li>
      </ul>
    </div>
  </nav>

    <NuxtPage />
  
  </div>
</template>
