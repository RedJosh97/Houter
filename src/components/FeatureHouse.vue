<template>
  <div class="feature-section">
    <HousingProps
      title="woodlandside"
      amount="$ 20.000.00"
      profilePicture=""
      name="Robert Fox"
      description="Dr. San Jane South Dakota"
    />
    <div class="feature">
      <div class="feature-style">
        <HeadlineProps subTitle="Our Recomendation" title="FeatureHouse" />
      </div>
      <div class="feature-house-btn">
        <div class="select-btn">
          <button class="btn"><img src="/public/images/ph_house-fill.png" /> House</button>
          <button class="btn"><img src="/public/images/ic_round-villa.png" />Villa</button>
          <button class="btn"><img src="/public/images/ic_round-apartment.png" />Apartment</button>
          <div class="btn-side">
            <button class="btn-side-left"><i class="las la-angle-left"></i></button>
            <button class="btn-side-right"><i class="las la-angle-right"></i></button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import HousingProps from './HousingProps.vue'

export default {
  name: 'FeatureHouse',
  components: { HeadlineProps, HousingProps }
}
</script>

<style scoped>
.feature {
  padding-top: 5rem;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.feature-house-btn {
  display: flex;
  justify-content: center;
  align-items: center;
}

.select-btn {
  /* padding-left: 100px; */
  display: flex;
  gap: 3%;
}
.btn:hover {
  background: var(--light-color);
  color: var(--deep-color);
}
.select-btn img:hover {
  background: transparent;
}

.btn {
  display: flex;
  align-items: center;
  padding: 0.7rem 1.5rem;
  border-radius: 32px;
  /* gap: 0.3rem; */
  gap: 3%;
  background: transparent;
  border: 1px solid #e0e3eb;
}

.btn-side {
  gap: 16px;
  display: flex;
}
.btn-side button {
  border: none;
  padding: 16px 16px;
  border-radius: 27px;
  background: var(--deep-color);
  color: #fff;
}
</style>
