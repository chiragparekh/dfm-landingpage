<template>
  <div id="app">
    <Header />
    <Hero />
    <div class="container mx-auto px-4">
      <!-- <div class="w-full md:w-5/6 md:mx-auto"> -->
        <FindPartner />
        <Features />
        <FindSection />
        <SubscribeSection />
      <!-- </div> -->
      <Footer />
    </div>
  </div>
</template>

<script>
import Header from '@/components/Header.vue'
import Footer from '@/components/Footer.vue'
import Hero from '@/components/Hero.vue'
import FindSection from '@/components/FindSection.vue'
import FindPartner from '@/components/FindPartner.vue'
import SubscribeSection from '@/components/SubscribeSection.vue'
import Features from '@/components/Features.vue'

export default {
  name: 'App',
  components: {
    Header,
    Footer,
    Hero,
    FindSection,
    FindPartner,
    SubscribeSection,
    Features,
  }
}
</script>