<template>
  <div class="bg-gray-200 w-full z-50">
    <div class="mx-auto flex items-center justify-center flex-col md:flex-row">
      <div class="flex items-center justify-center md:justify-start pt-5">
        <NuxtLink to="/" class="hover:underline non-italic">
          <nuxt-img
            src="/icologo.png"
            alt="Logo"
            class="h-10 md:h-16"
            sizes="sm:100vw md:50vw lg:1500px "
            format="webp"
          />
        </NuxtLink>
      </div>
    </div>
    <div class="mx-auto">
      <p class="text-md text-gray-600 font-serif italic text-center">
        "Empowering User Experience through Code Craftsmanship."
      </p>
      <p class="text-sm text-gray-400 text-center mt-4 pb-10">
        &copy; 2023. Aysegulk.me All Rights Reserved.
      </p>
      <hr class="border-gray-300 mx-auto pb-10" />
    </div>
  </div>
</template>
