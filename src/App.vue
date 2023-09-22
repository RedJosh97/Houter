<template>
  <div>
    <NavBar />
    <HeroSection />
    <FeatureHouse />
    <TourHousing />
  </div>
</template>

<script>
import NavBar from './components/NavBar.vue'
import HeroSection from './components/HeroSection.vue'
import FeatureHouse from './components/FeatureHouse.vue'
import TourHousing from './components/TourHousing.vue'

export default {
  name: 'App',
  components: {
    NavBar,
    HeroSection,
    FeatureHouse,
    TourHousing
  }
}
</script>

<style scoped></style>
