<style>
@import url('https://fonts.googleapis.com/css2?family=Jersey+15&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Press+Start+2P&display=swap');


.jersey-font {
  font-family: 'Jersey 15', sans-serif;
}
.undertale-battle-font {
  font-family: "Undertale_Battle_Font", system-ui;
  font-weight: 400;
  font-size: 2.5rem;
  font-style: normal;

}
@font-face {
	font-family: 'Undertale_Battle_Font';
	src: url('../fonts/undertale_battle_font.eot'); /* IE 9 Compatibility Mode */
	src: url('../fonts/undertale_battle_font.eot?#iefix') format('embedded-opentype'), /* IE < 9 */
		url('../fonts/undertale_battle_font.woff2') format('woff2'), /* Super Modern Browsers */
		url('../fonts/undertale_battle_font.woff') format('woff'), /* Firefox >= 3.6, any other modern browser */
		url('../fonts/undertale_battle_font.ttf') format('truetype'), /* Safari, Android, iOS */
		url('../fonts/undertale_battle_font.svg#undertale_battle_font') format('svg'); /* Chrome < 4, Legacy iOS */
}

</style>
<script setup>
import { useI18n } from 'vue-i18n'
import { ref, watch, onMounted } from 'vue'

const { locale, locales, setLocale } = useI18n()


function handleChange(event) {
  const newLocale = event.target.value
  setLocale(newLocale)
  localStorage.setItem('locale', newLocale)
}
onUpdated(() => {
  const saved = localStorage.getItem('locale')
  if (saved && saved !== locale.value) {
      setLocale(saved)
    }
})
</script>
<template>
  <main :class="locale === 'ru' ? 'undertale-battle-font' : 'jersey-font'">
    <div class="background">
      <header class ='flex flex-row items-center w-full bg-[#aab597] border-b-[7px] border-t-[7px] border-[#475e47]'>
        <div class="basis-1/4 items-center justify-start px-8">
          <NuxtLink to="/">
            <img src="assets/images/Runaways_Logo.svg" class="w-20 h-auto hover:bg-[#475e47] rounded-full p-2 max-[600px]:p-0 transition-all duration-60">
          </NuxtLink>
        </div>
        <div class="basis-1/2 flex flex-row justify-center max-[600px]:pl-8 text-center">
          <h1 class=" flex flex-row jersey-font text-8xl text-[#fafaee] max-[600px]:text-6xl hover:text-9xl transition-all duration-300">Runaways</h1>
        </div>
        <nav class="basis-1/4 max-[600px]:hidden flex flex-row items-center justify-end px-8 gap-4">
          <NuxtLink to="/Creators" class="my-auto text-5xl text-[#fafaee] p-2 hover:text-[#c7dec7] hover:bg-[#475e47] rounded-2xl transition-all duration-60">{{$t('creators')}}</NuxtLink>
        </nav>
      </header>
      <main class="flex flex-col h-auto">
        <slot />
      </main>
      <footer class="flex flex-row w-full bg-[#aab597] border-b-[7px] border-t-[7px] border-[#475e47] items-center justify-center px-4 py-10 gap-4">
        <!--a href="https://www.youtube.com/"><img src="assets/images/youtube_logo.svg" class="w-16 h-16 hover:bg-[#1b2028]"></a>
        <a href="https://github.com/"><img src="assets/images/github_logo.svg" class="w-16 h-16 hover:bg-[#1b2028]"></a-->
          <div>
            <select @change="handleChange" :value="locale" class=" p-1 items-center rounded bg-[#475e47] text-2xl  text-[#fafaee]">
            <option value="en">English</option>
            <option value="ru">Русский</option>
          </select>
    
          </div>
      </footer>
    </div>
  </main>
  </template>
  
  <style>
  .background {
    background: url("assets/images/Runaways_BG_1.webp") repeat;
    background-size: 75%;
    image-rendering: pixelated;
  }
  </style>