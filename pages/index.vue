<template>
  <main class="custom-bg flex flex-col items-center min-h-[95vh] py-10 rounded-2xl justify-between">
    <div class="flex-grow"></div> 
    <div class="bg-[#6b8f6b] p-8 rounded-2xl shadow-lg max-w-3xl w-full mx-auto">
      <h1 class="jersey-font text-7xl text-[#fafaee] text-center">Choose who you want to know more about:</h1>
      <NuxtLink to="/Morozov_Sergey" class="jersey-font text-5xl text-[#fafaee] hover:text-[#6b8f6b] hover:bg-[#c7dec7] hover:text-6xl rounded-2xl transition-all duration-300 block p-2">
        ● Morozov Sergey
      </NuxtLink>
      <NuxtLink to="/Artyom_Zaichenko" class="jersey-font text-5xl text-[#fafaee] hover:text-[#6b8f6b] hover:bg-[#c7dec7] hover:text-6xl rounded-2xl transition-all duration-300 block p-2">
        ● Artyom Zaichenko
      </NuxtLink>
      <NuxtLink to="/Oleinikov_Danila" class="jersey-font text-5xl text-[#fafaee] hover:text-[#6b8f6b] hover:bg-[#c7dec7] hover:text-6xl rounded-2xl transition-all duration-300 block p-2">
        ● Oleinikov Danila
      </NuxtLink>
    </div>
    <div class="flex-grow"></div> 
  </main>
</template>

<style>
.custom-bg {
  background: url('assets/images/Runaways_BG_3.webp') repeat;
  background-size: 40%;
  image-rendering: pixelated;
}
</style>