<template>
  <main class="custom-bg flex flex-col items-center min-h-[95vh] py-10 justify-between">
    <div class="flex-grow"></div> 
    <div class="bg-[#6b8f6b] p-8 rounded-2xl shadow-lg max-w-3xl w-full mx-auto">
      <h1 class=" text-7xl text-[#fafaee] text-center">{{ $t('creators')}}</h1>
      <p class=" text-5xl text-[#fafaee] text-center">{{ $t('namems')}}</p>
      <p class=" text-5xl text-[#fafaee] text-center">{{ $t('nameaz')}}</p>
      <p class=" text-5xl text-[#fafaee] text-center">{{ $t('nameod')}}</p>
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