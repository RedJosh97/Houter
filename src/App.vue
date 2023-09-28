<template>
  <div>
    <NavBar />
    <HeroSection />
    <FeatureHouse />
    <TourHousing />
    <TimeLineArticle />
    <SellingHome />
    <SubscribeLayout />
    <FooterSection />
  </div>
</template>

<script>
import NavBar from './components/NavBar.vue'
import HeroSection from './components/HeroSection.vue'
import FeatureHouse from './components/FeatureHouse.vue'
import TourHousing from './components/TourHousing.vue'
import FooterSection from './components/FooterSection.vue'
import SellingHome from './components/SellingHome.vue'
import TimeLineArticle from './components/TimelineArticle.vue'
import SubscribeLayout from './components/SubscribeLayout.vue'

export default {
  name: 'App',
  components: {
    NavBar,
    HeroSection,
    FeatureHouse,
    TourHousing,
    TimeLineArticle,
    FooterSection,
    SellingHome,
    SubscribeLayout
  }
}
</script>

<style scoped></style>
