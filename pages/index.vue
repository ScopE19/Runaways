<script setup>
const { locales, setLocale } = useI18n()
</script>
<template>
  <main class="custom-bg flex flex-col items-center min-h-[95vh] py-10 justify-between">
    <div class="flex-grow"></div> 
    <div class="bg-[#6b8f6b] p-8 rounded-2xl shadow-lg max-w-3xl w-full h-auto mx-auto">
      <h1 class=" text-[#fafaee] text-center text-7xl">{{ $t('choose') }}</h1>
      <NuxtLink to="/Morozov_Sergey" class=" text-5xl text-[#fafaee] hover:text-[#6b8f6b] hover:bg-[#c7dec7] hover:text-6xl rounded-2xl transition-all duration-300 block p-2">
        {{ $t('sergey_index') }}
      </NuxtLink>
      <NuxtLink to="/Artyom_Zaichenko" class=" text-5xl text-[#fafaee] hover:text-[#6b8f6b] hover:bg-[#c7dec7] hover:text-6xl rounded-2xl transition-all duration-300 block p-2">
        {{ $t('artyom_index') }}
      </NuxtLink>
      <NuxtLink to="/Oleinikov_Danila" class="text-5xl text-[#fafaee] hover:text-[#6b8f6b] hover:bg-[#c7dec7] hover:text-6xl rounded-2xl transition-all duration-300 block p-2">
        {{ $t('danila_index') }}
      </NuxtLink>
    </div>
    <div class="flex-grow"></div> 
  </main>
</template>

<style>
.custom-bg {
  background: url('assets/images/Runaways_BG_4_1.webp') repeat;
  background-size: 50%;
  image-rendering: pixelated;
}
</style>