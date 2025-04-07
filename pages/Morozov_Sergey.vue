
<template>
  <main class="custom-bg flex flex-col items-center min-h-[95vh] py-10 justify-between'">
    <div class="flex-grow"></div> 
    <div class="bg-[#6b8f6b] p-6 rounded-2xl shadow-lg max-w-5xl w-full h-auto mx-auto">
      <h1 class=" text-7xl text-[#fafaee] text-center mb-6">{{ $t('namems')}}</h1>
      <div class="flex flex-col md:flex-row items-center gap-6">
        <img src="assets/images/Sergey_photo.png" alt="Morozov Sergey" class="w-64 h-auto rounded-2xl shadow-lg hover:w-80 transition-all duration-300">
        <div class="text-[#fafaee] text-xl flex-1">
          <p class=" mb-4 text-4xl text-[#c7dec7] max-h-[90vh]">
            {{ $t('basic_info') }}
          </p>
          <p class=" mb-4 text-2xl text-[#fafaee] max-h-[90vh]">
            {{ $t('basic_info_sergey') }}
          </p>
          <p class=" mb-4 text-4xl text-[#c7dec7] max-h-[90vh]">
            {{ $t('summary') }}
          </p>
          <p class=" mb-4 text-2xl text-[#fafaee] max-h-[90vh]">
            {{ $t('summary_sergey') }}
          </p>
        </div>
      </div>
      <div class="mt-6 ">
        <p class=" mb-4 text-4xl text-[#c7dec7] max-h-[90vh]">{{ $t('additional_info')}}</p>
        <p class=" mb-4 text-2xl text-[#fafaee] max-h-[90vh]">
          {{ $t('additional_info_sergey') }}
        </p>
        <p class=" mb-4 text-2xl text-[#fafaee] max-h-[90vh]">
          {{ $t('additional_info_sergey_2') }}
        </p>
      </div>
    </div>
    <div class="flex-grow"></div> 
  </main>
</template>

<style>
.custom-bg {
  background: url('assets/images/Runaways_BG_4.webp') repeat;
  background-size: 50%;
  image-rendering: pixelated;
}
</style>