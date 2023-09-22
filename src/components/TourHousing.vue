<template>
  <div class="lets-tour-container">
    <div class="tour-wrapper">
      <HeadlineProps subTitle="Ready to sell!!" title="Let's Tour and see our House!" />
      <div class="tour-wrapper-left">
        <div class="house-details">
          <p class="details-text">House Detail</p>
          <div class="house-product-wrapper">
            <div class="house-details-product">
              <img src="/public/images/bed 1.png" />
              <p>4 bedroom</p>
            </div>
            <div class="house-details-product">
              <img src="/public/images/bath 1.png" />
              <p>2 bathroom</p>
            </div>
            <div class="house-details-product">
              <img src="/public/images/car-garage 1.png" />
              <p>1 carper</p>
            </div>
            <div class="house-details-product">
              <img src="/public/images/stairs-with-handrail 1.png" />
              <p>2 floor</p>
            </div>
          </div>
          <div class="tour-profile-container">
            <img src="/public/images/Ellipse 6-2.png" />
            <div class="profile-content">
              <p class="cont-name">Dianne Rossele</p>
              <p>Manager Director</p>
            </div>
            <button class="contact-box-btn"><i class="las la-phone"></i>Contact now</button>
          </div>
        </div>
      </div>
    </div>
    <div class="container-left-right"></div>
    <div class="tour-wrapper-right">
      <img class="play-button" src="/public/images/bi_play-circle-fill.png" />
      <div class="tour-image-wrapper">
        <img src="/public/images/Rectangle 17.png" />
        <div class="small-house-container">
          <img class="rectangle-image" src="/public/images/Rectangle 18.png" />
          <img src="/public/images/Rectangle 19.png" />
          <img src="/public/images/Rectangle 20.png" />
        </div>
      </div>
    </div>
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
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.container-left-right {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.tour-wrapper-left {
  max-width: 380px;
}
.house-details .details-text {
  font-weight: 700;
  padding-top: 16px;
}
.house-details p {
  color: var(--par-color);
}

.house-product-wrapper {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
}
.profile-content .cont-name {
  color: var(--head-color);
}
.tour-profile-container {
  display: flex;
  align-items: center;
  gap: 18px;
  border-radius: 3px;
  padding-top: 48px;
}
.tour-wrapper-right {
  position: relative;
}
.tour-image-wrapper img {
  width: 100%;
}

.small-house-container .rectangle-image {
  height: 120px;
  background: green;
}
.play-button {
  transform: translateX(450%) translateY(450%);
  width: 10%;
}
.small-house-container {
  display: flex;
  justify-content: space-between;
  align-items: end;
  gap: 12px;
  width: 70%;
  height: 140px;
  position: absolute;
  transform: translateX(-9%) translateY(-80%);
}
.small-house-container img {
  object-fit: cover;
  height: 70%;
}
.contact-box-btn {
  display: inline-flex;
  padding: 12px 16px;
  align-items: center;
  gap: 16px;
  background: var(--deep-color);
  color: #fff;
  border: none;
  border-radius: 32px;
}
</style>
