<template>
  <div class="h-[10%] flex justify-center items-center">
    <span class="text-2xl font-bold tracking-wide">MyHotel</span>
  </div>
  <div class="w-full h-[90%] px-5">
    <NuxtLink
      to="/"
      :class="$route.path === '/' ? 'text-white bg-black' : 'text-black'"
      class="w-full flex py-2 px-4 rounded-md mb-1"
    >
      Home
    </NuxtLink>
    <NuxtLink
      to="/about"
      :class="$route.path === '/about' ? 'text-white bg-black' : 'text-black'"
      class="w-full flex py-2 px-4 rounded-md mb-1"
    >
      About
    </NuxtLink>
  </div>
</template>
