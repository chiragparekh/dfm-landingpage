<style lang="scss" scoped>
.hero-section {
  margin-bottom: 200px;
}
.slider-wrapper {
  padding-top: 700px;
}
.desktop-slider {
  height: 700px;
}
/* prefix with transition name */
.slide-fade-enter-active {
  opacity: 1;
  z-index: 10;
}

.slide-fade-leave-active {
  opacity: 1;
}

.slide-fade-enter,
.slide-fade-leave-to {
  opacity: 0;
}
.slide-image {
  height: 700px;
  background-color: #cecece;
  -webkit-transition: all 0.8s ease;
  transition: all 0.8s ease;
}
@media screen and (max-width: 768px) {
  .hero-section {
    margin-bottom: 180px;
  }
  .slider-wrapper {
    padding-top: 500px;
  }
  .slide-image {
    height: 500px;
  }
}
@media screen and (max-width: 425px) {
  .hero-section {
    margin-bottom: 0px;
  }
  .desktop-slider {
    height: 350px;
  }
  .slider-wrapper {
    padding-top: 0;
  }
  .slide-image {
    height: 350px;
  }
}
</style>
<template>
  <div class="hero-section">
    <div class="relative slider-wrapper">
      <div class="desktop-slider relative md:top-0 md:w-full md:absolute">
        <div class="container mx-auto relative">
          <transition name='slide-fade'>
              <div :key='currentIndex' :style="{'background-image': `url(${currentImg['image']})`}" class="absolute left-0 w-full h-full slide-image bg-cover bg-center bg-no-repeat">
                <div class="hidden border-t-4 border-siteRed-700 bg-white bg-opacity-95 py-4 px-2 absolute z-10 bottom-0 right-0 mr-56 mb-32 w-1/4 lg:block">
                  <p class="text-xs text-center text-gray-600 mb-4">{{ currentImg['person']['quote'] }}</p>
                  <p class="text-xs font-bold text-center text-gray-500">{{ currentImg['person']['name'] }} {{ currentImg['person']['age'] }} | {{ currentImg['person']['city'] }}</p>
                </div>
              </div>
          </transition>
        </div>
      </div>
      <div class="relative w-full left-0 top-0 z-10 -mt-6 sm:absolute sm:mt-auto">
        <div class="container mx-auto sm:pt-10 sm:pb-32 sm:mt-0 lg:pt-20">
          <div class="px-4 flex w-full md:w-5/6 md:mx-auto">
            <div class="flex flex-col bg-siteBlue-900 text-white p-2 mt-0 rounded md:mt-12 md:w-1/2 lg:w-1/3">
              <h2 class="text-center text-lg mb-6">Über 1 Millionen Singles warten auf Dich- Online Dating mit unserer Singlebörse.</h2>
              <label class="text-xs font-bold">Kostenlos registrieren</label>
              <input type="text" placeholder="Email" class="px-4 py-3 mt-1 rounded text-center text-gray-700 mb-1 text-sm focus:outline-none">
              <button type="button" class="px-4 py-3 w-full bg-siteRed-700 rounded my-2 text-sm font-bold">Jetzt registrieren</button>
              <p class="text-2xs mb-4">Mit dem Klick auf „Jetzt registrieren“ stimme ich den AGB und Datenschutzbestimmungen zu.</p>
              <button type="button" class="px-4 py-3 w-full bg-siteRed-800 rounded my-2 text-sm focus:outline-none font-bold">Login</button>
            </div>
          </div>
        </div>
      </div>
      <div class="relative z-10 w-full sm:absolute">
        <div class="container mx-auto sm:-my-10">
          <div class="hero-items my-4 px-4 md:w-5/6 md:mx-auto">
            <div class="flex -mx-2">
              <div class="item w-1/3 flex flex-col px-2">
                <div class="bg-gray-200 flex justify-center items-center flex-col h-full pt-4 pb-8 md:py-10">
                  <span>
                    <svg class="w-10 h-10 text-gray-400 md:w-16 md:h-16" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                      <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z" />
                    </svg>
                  </span>
                  <h1 class="text-2xs text-center text-gray-600 mt-2 px-2 md:text-xs">Alle Profile pefrüft</h1>
                </div>
              </div>
              <div class="item w-1/3 flex flex-col px-2">
                <div class="bg-gray-200 flex justify-center items-center flex-col h-full pt-4 pb-8">
                  <span>
                    <svg class="w-10 h-10 text-gray-400 md:w-16 md:h-16" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                      <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 20h5v-2a3 3 0 00-5.356-1.857M17 20H7m10 0v-2c0-.656-.126-1.283-.356-1.857M7 20H2v-2a3 3 0 015.356-1.857M7 20v-2c0-.656.126-1.283.356-1.857m0 0a5.002 5.002 0 019.288 0M15 7a3 3 0 11-6 0 3 3 0 016 0zm6 3a2 2 0 11-4 0 2 2 0 014 0zM7 10a2 2 0 11-4 0 2 2 0 014 0z" />
                    </svg>
                  </span>
                  <h1 class="text-2xs text-center text-gray-600 mt-2 px-2 md:text-xs">Mehr als 1.000 neue Mitglieder jeden Tag</h1>
                </div>
              </div>
              <div class="item w-1/3 flex flex-col px-2">
                <div class="bg-gray-200 flex justify-center items-center flex-col h-full pt-4 pb-8">
                  <svg class="w-10 h-10 text-gray-400 md:w-16 md:h-16" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m5.618-4.016A11.955 11.955 0 0112 2.944a11.955 11.955 0 01-8.618 3.04A12.02 12.02 0 003 9c0 5.591 3.824 10.29 9 11.622 5.176-1.332 9-6.03 9-11.622 0-1.042-.133-2.052-.382-3.016z" />
                  </svg>
                  <h1 class="text-2xs text-center text-gray-600 mt-2 px-2 md:text-xs">Datenübertragung per sicherer SSL Verbindung</h1>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import image1 from '../assets/images/woman_slider@2x.png'
import image2 from '../assets/images/man_slider@2x.png'

export default {
  name: 'Hero',
  data() {
    return {
      show: false,
      images: [
        {
          image: image1,
          person: {
            name: 'Steffi',
            age: '32',
            quote: '„Mein Partner sollte mit beiden Beinen im Leben stehen.“',
            city: 'Düsseldorf',
          }
        },
        {
          image: image2,
          person: {
            name: 'Dummy',
            age: '33',
            quote: '„Some quot from the dummy person.“',
            city: 'Düsseldorf',
          }
        },
        // "https://cdn.pixabay.com/photo/2016/02/17/23/03/usa-1206240_1280.jpg",
        // "https://cdn.pixabay.com/photo/2015/05/15/14/27/eiffel-tower-768501_1280.jpg",
        // "https://cdn.pixabay.com/photo/2016/12/04/19/30/berlin-cathedral-1882397_1280.jpg"
      ],
      timer: null,
      currentIndex: 0
    };
  },
  mounted: function() {
    this.startSlide();
  },

  methods: {
    startSlide: function() {
      this.timer = setInterval(this.next, 3000);
    },

    next: function() {
      this.show = !this.show
      this.currentIndex += 1;
      if(this.currentIndex == this.images.length)
        this.currentIndex = 0
    },
    prev: function() {
      this.currentIndex -= 1;
      if(this.currentIndex == -1)
        this.currentIndex = 0
    }
  },

  computed: {
    currentImg: function() {
      return this.images[this.currentIndex];
    }
  }
}
</script>