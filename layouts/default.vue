<style>
@import url('https://fonts.googleapis.com/css2?family=Jersey+15&display=swap');

.jersey-font {
  font-family: 'Jersey 15', sans-serif;
}
</style>
<template>
    <div class="background">
      <header class="flex flex-row items-center w-full bg-[#aab597] border-b-[7px] border-t-[7px] border-[#475e47]">
        <div class="basis-1/4 items-center justify-start px-8">
          <NuxtLink to="/">
            <img src="assets/images/Runaways_Logo.svg" class="w-20 h-auto hover:bg-[#475e47] rounded-full p-2 max-[600px]:p-0 transition-all duration-60">
          </NuxtLink>
        </div>
        <div class="basis-1/2 text-center">
          <h1 class="jersey-font text-8xl text-[#fafaee] hover:text-9xl transition-all duration-300">Runaways</h1>
        </div>
        <nav class="basis-1/4 max-[600px]:hidden flex flex-row items-center justify-end px-8 gap-4">
          <NuxtLink to="/Creators" class="jersey-font my-auto text-5xl text-[#fafaee] p-2 hover:text-[#c7dec7] hover:bg-[#475e47] rounded-2xl transition-all duration-60">Creators</NuxtLink>
        </nav>
      </header>
      <main class="flex flex-col h-auto">
        <slot />
      </main>
      <footer class="flex flex-row w-full bg-[#aab597] border-b-[7px] border-t-[7px] border-[#475e47] items-center justify-center px-4 py-10 gap-4">
        <!--a href="https://www.youtube.com/"><img src="assets/images/youtube_logo.svg" class="w-16 h-16 hover:bg-[#1b2028]"></a>
        <a href="https://github.com/"><img src="assets/images/github_logo.svg" class="w-16 h-16 hover:bg-[#1b2028]"></a-->
      </footer>
    </div>
  </template>
  
  <style>
  .background {
    background: url("assets/images/Runaways_BG_1.webp") repeat;
    background-size: 75%;
    image-rendering: pixelated;
  }
  </style>