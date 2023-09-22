<template>
  <div class="lets-tour-container">
    <div class="tour-wrapper">
      <HeadlineProps subTitle="Ready to sell!!" title="Let's Tour and see our House!" />
    </div>
    <div class="tour-wrapper-left"></div>
    <div class="tour-wrapper-right"></div>
  </div>
</template>

<script>
import HeadlineProps from './HeadlineProps.vue'

export default {
  name: 'TourHousing',
  components: { HeadlineProps }
}
</script>

<style scoped>
.lets-tour-container {
  padding-top: 120px;
}
</style>
