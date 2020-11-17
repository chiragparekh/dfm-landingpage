<style lang="scss" scoped>
  .custom-bg-image {
    background-image: url('../assets/images/man_mobile@2x.png');
  }
  @media screen and (max-width: 767px) {
    .custom-bg-image {
      background-image: none;
    }
  }
</style>
<template>
  <div class="find-partner -mx-4 md:my-16">
    <div class="px-4 md:mb-10">
      <h1 class="text-xl text-center text-gray-500 mb-3 sm:text-4xl sm:font-semibold">Chatten, Flirten, Daten<br/>Finde Deinen Partner</h1>
      <div class="flex justify-center">
        <svg class="w-6 h-6 fill-current text-siteRed-900 md:w-10 md:h-10" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4.318 6.318a4.5 4.5 0 000 6.364L12 20.364l7.682-7.682a4.5 4.5 0 00-6.364-6.364L12 7.636l-1.318-1.318a4.5 4.5 0 00-6.364 0z" />
        </svg>
      </div>
      <h3 class="text-center my-2 text-lg text-gray-500 sm:text-2xl sm:font-semibold">Wo und wann du willst</h3>
    </div>
    <div class="bg-cover bg-no-repeat custom-bg-image sm:bg-right-top">
      <div class="w-full md:w-5/6 md:mx-auto">
        <div class="w-full lg:w-1/2">
          <img src="@/assets/images/man_mobile@2x.png" class="block sm:hidden">
          <div class="items flex flex-wrap px-4 -mx-2 justify-center -mt-8 md:mt-0">
            <div class="item-wrapper w-1/2 px-2">
              <div class="item bg-white border-t-8 border-siteRed-900 mb-4 px-2 py-4 bg-opacity-75">
                <div class="flex justify-center mb-4">
                  <svg class="w-10 h-10 text-blue-800" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z" />
                  </svg>
                </div>
                <h3 class="text-center text-sm mb-1">Kostenlose Anmeldung</h3>
                <p class="text-xs text-center">In einer Minute anmelden und über eine Millionen Singles finden.</p>
              </div>
            </div>
            <div class="item-wrapper w-1/2 px-2">
              <div class="item bg-white border-t-8 border-siteRed-900 mb-4 px-2 py-4 bg-opacity-75">
                <div class="flex justify-center mb-4">
                  <svg class="w-10 h-10 text-blue-800" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" />
                  </svg>
                </div>
                <h3 class="text-center text-sm mb-1">Nachrichten schreiben</h3>
                <p class="text-xs text-center">Mit deinem Smartphone von überall immer im Kontakt bleiben.</p>
              </div>
            </div>
            <div class="item-wrapper w-1/2 px-2">
              <div class="item bg-white border-t-8 border-siteRed-900 mb-4 px-2 py-4 bg-opacity-75">
                <div class="flex justify-center mb-4">
                  <svg class="w-10 h-10 text-blue-800" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor">
                    <path fill-rule="evenodd" d="M5 9V7a5 5 0 0110 0v2a2 2 0 012 2v5a2 2 0 01-2 2H5a2 2 0 01-2-2v-5a2 2 0 012-2zm8-2v2H7V7a3 3 0 016 0z" clip-rule="evenodd" />
                  </svg>
                </div>
                <h3 class="text-center text-sm mb-1">Völlig anonym</h3>
                <p class="text-xs text-center">Verschlüsselte Daten für die maximale Privatsphäre.</p>
              </div>
            </div>
            <div class="item-wrapper w-1/2 px-2">
              <div class="item bg-white border-t-8 border-siteRed-900 mb-4 px-2 py-4 bg-opacity-75">
                <div class="flex justify-center mb-4">
                  <svg class="w-10 h-10 text-blue-800" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor">
                    <path d="M9 9a2 2 0 114 0 2 2 0 01-4 0z" />
                    <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm1-13a4 4 0 00-3.446 6.032l-2.261 2.26a1 1 0 101.414 1.415l2.261-2.261A4 4 0 1011 5z" clip-rule="evenodd" />
                  </svg>
                </div>
                <h3 class="text-center text-sm mb-1">Echte Frauen und Männer</h3>
                <p class="text-xs text-center">Geprüfte Profile und Bilder für seriöse Kontakte.</p>
              </div>
            </div>
          </div>
          <div class="flex flex-wrap px-4 -mx-2 my-10 justify-center md:my-2">
            <div class="relative h-56 w-56 sm:h-64 sm:w-64">
              <div class="shadow absolute transform -rotate-12">
                <div class="w-56 h-56 bg-cover bg-no-repeat relative sm:h-64 sm:w-64"
                  :style="{'background-image': `url('${require('@/assets/images/couple01@2x.png')}')`}"
                >
                  <div class="flex items-center bg-white opacity-75 absolute bottom-0 left-0 w-full px-1 py-1 text-gray-600">
                    <h3 class="w-1/2 font-bold text-xs truncate">Sunny-Lucie</h3>
                    <ul class="w-1/2 flex text-2xs items-center ml-auto">
                      <li class="mr-1">32 Jahre</li>
                      <li class="pl-1 mr-1 border-l">Berline</li>
                      <li class="pl-1 border-l">9.6 km</li>
                    </ul>
                  </div>
                </div>
              </div>
              <div class="shadow absolute">
                <div class="w-56 h-56 bg-cover bg-no-repeat relative sm:h-64 sm:w-64"
                  :style="{'background-image': `url('${require('@/assets/images/couple02@2x.png')}')`}"
                >
                  <div class="flex items-center bg-white opacity-75 absolute bottom-0 left-0 w-full px-1 py-1 text-gray-600">
                    <h3 class="w-1/2 font-bold text-xs truncate">Sunny-Lucie</h3>
                    <ul class="w-1/2 flex text-2xs items-center ml-auto">
                      <li class="mr-1">32 Jahre</li>
                      <li class="pl-1 mr-1 border-l">Berline</li>
                      <li class="pl-1 border-l">9.6 km</li>
                    </ul>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>