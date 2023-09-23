<template>
  <div>
    <NavBar />
    <HeroSection />
    <FeatureHouse />
    <TourHousing />
    <TimeLineArticle />
  </div>
</template>

<script>
import NavBar from './components/NavBar.vue'
import HeroSection from './components/HeroSection.vue'
import FeatureHouse from './components/FeatureHouse.vue'
import TourHousing from './components/TourHousing.vue'
import TimeLineArticle from './components/TimelineArticle.vue'

export default {
  name: 'App',
  components: {
    NavBar,
    HeroSection,
    FeatureHouse,
    TourHousing,
    TimeLineArticle
  }
}
</script>

<style scoped></style>
