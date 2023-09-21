<template>
  <div>
    <NavBar />
    <HeroSection />
    <FeatureHouse />
  </div>
</template>

<script>
import NavBar from './components/NavBar.vue'
import HeroSection from './components/HeroSection.vue'
import FeatureHouse from './components/FeatureHouse.vue'

export default {
  name: 'App',
  components: {
    NavBar,
    HeroSection,
    FeatureHouse
  }
}
</script>

<style scoped></style>
