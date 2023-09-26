<template>
  <div class="headline">
    <img class="cliper" src="/public/images/Vector (3).png" />
    <img class="cliper2" src="/public/images/Vector (4).png" />
    <HeadlineProps
      title="Find out more about selling and buying homes"
      subTitle="See key and tips for our
    partnership"
    >
      <template #displayOther>
        <button class="contact-box-btn">More article</button>
      </template>
    </HeadlineProps>
  </div>
  <div class="selling-home-container">
    <div class="sell-left-section">
      <SellSectionProps
        :picture="'/public/images/Rectangle 22-1.png'"
        :smallPix="'/public/images/Ellipse 6-1.png'"
        content="7 Ways to distinguish the quality of the house we want to buy"
        name="Courtney Henry"
        timeline="16 min read | 7 April 2023"
      />
      <SellSectionProps
        :picture="'/public/images/Rectangle 22-2.png'"
        :smallPix="'/public/images/Ellipse 6.png'"
        content="The things we need to check when we want to buy a house"
        name="Dianne Rusell"
        timeline="16 min read | 7 April 2023"
      />
      <SellSectionProps
        :picture="'/public/images/Rectangle 22.png'"
        :smallPix="'/public/images/Ellipse 6-3.png'"
        content="The best way to know the quality of the house we want to buy"
        name="Darlene Robertson"
        timeline="16 min read | 7 April 2023"
      />
      <SellSectionProps
        :picture="'/public/images/Rectangle 22.png'"
        :smallPix="'/public/images/Ellipse 6-3.png'"
        content="The best way to know the quality of the house we want to buy"
        name="Darlene Robertson"
        timeline="16 min read | 7 April 2023"
      />
    </div>

    <!-- <div class="sell-right-section">
      <img class="sell-picture-right" src="/public/images/Rectangle 23.png" />
      <div class="profile-wrapper">
        <img class="small-profile-pix" src="/public/images/Ellipse 6.png" />
        <p>Cameroon Williamson</p>
      </div>
      <p class="title">12 Things to know before buying a house</p>
      <p>
        Want to buy a house but are unsure about what we should know, here I will try to explain
        what we should know and check when we want to buy a house
      </p>
      <div class="min-ago">
        <i class="las la-clock"></i>
        <p>18 min read | 5 June 2021</p>
      </div>
    </div> -->
  </div>
</template>

<script>
import HeadlineProps from './HeadlineProps.vue'
import SellSectionProps from './SellSectionProps.vue'

export default {
  name: 'SellingHome',
  components: { SellSectionProps, HeadlineProps }
}
</script>

<style>
.cliper {
  position: absolute;
  top: -220px;
  left: -490px;
  z-index: -40;
}
.cliper2 {
  position: absolute;
  top: 20px;
  left: -520px;
  z-index: -50;
}

.headline {
  text-align: center;
  margin: 42px auto;
  max-width: 422px;
  position: relative;
}
.sell-left-section {
  display: flex;
  flex-direction: column;
  gap: 42px;
}

.selling-home-container {
  display: flex;
  gap: 68px;
  justify-content: space-between;
  flex: 2;
}
.selling-home-container p {
  color: var(--par-color);
  font-size: 13px;
}
.small-profile-pix {
  width: 25px;
}
.sell-right-section .title {
  color: var(--head-color);
  font-size: 1.2rem;
}
/* .sell-right-section {
  max-width: 560px;
  display: flex;
  gap: 12px;
  flex-direction: column;
} */

/* .sell-picture-right {
  width: 100%;
  border-radius: 14px;
} */

.profile-wrapper {
  display: flex;
  align-items: center;
  gap: 16px;
}

.la-clock {
  margin-right: 12px;
}
.min-ago {
  display: flex;
}
</style>
