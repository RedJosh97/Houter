<template>
  <div class="lets-tour-container">
    <div class="tour-wrapper">
      <HeadlineProps subTitle="Ready to sell!!" title="Let's Tour and see our House!" />
      <div class="tour-wrapper-left">
        <div class="house-details">
          <p>
            Houses recommended by our partners that have been curated to become the home of your
            dreams!
          </p>
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
    <div class="tour-wrapper-right">
      <div class="imageg">
        <img class="play-button" src="/public/images/bi_play-circle-fill.png" />
      </div>
      <div class="tour-image-wrapper">
        <img class="clipper" src="/public/images/Vector (2).png" />
        <img class="billboard-image" src="/public/images/Rectangle 17.png" />
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

<style>
.lets-tour-container {
  padding: 80px 7rem 0;
  display: flex;
  gap: 12px;
  justify-content: space-between;
  align-items: center;
}
.container-left-right {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.tour-wrapper-left {
  max-width: 430px;
  min-width: 330px;
  margin-top: 2rem;
  display: flex;
  gap: 16px;
}
.house-details .details-text {
  font-weight: 700;
  padding-top: 16px;
}
.house-details p {
  color: var(--par-color);
}
.clipper {
  position: absolute;
  top: -270px;
  right: -120px;
  /* transform: translateX(118.9%) translateY(-47%); */
  overflow: hidden;
  z-index: -20;
}
.details-text {
  margin-bottom: 12px;
}
.house-product-wrapper {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  row-gap: 13px;
}
.profile-content .cont-name {
  color: var(--head-color);
}
.tour-profile-container {
  /* position: relative; */
  display: flex;
  align-items: center;
  flex-wrap: wrap;
  gap: 18px;
  border-radius: 3px;
  padding-top: 48px;
}
.tour-wrapper-right {
  position: relative;
}
.tour-image-wrapper {
  position: relative;
}
.tour-image-wrapper img {
  width: 100%;
}

.small-house-container .rectangle-image {
  height: 120px;
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
  height: 140px;
  position: absolute;
  transform: translateX(-9%) translateY(-80%);
}

.billboard-image {
  min-width: 330px;
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
