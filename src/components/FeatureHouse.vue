<template>
  <div class="feature-container-wrapper">
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
    <div class="housing-props-container">
      <HousingProps
        :building="'/public/images/Rectangle 15-2.png'"
        title="Roselands House"
        amount="$ 35. 000. 000"
        :profilePicture="'/public/images/Ellipse 6-2.png'"
        name="Dianne Rossele"
        description="Manchester Kentucky"
      />
      <HousingProps
        :building="'/public/images/Rectangle 15-1.png'"
        title="woodlandside"
        amount="$ 20. 000. 000"
        :profilePicture="'/public/images/Ellipse 6-1.png'"
        name="Robert Fox"
        description="Dr. San Jose, South Dakota"
      />
      <HousingProps
        :building="'/public/images/Rectangle 15-3.png'"
        title="The old ligth house"
        amount="$ 40. 000. 000"
        :profilePicture="'/public/images/Ellipse 6-3.png'"
        name="Roland Richards"
        description="Santa Ana, Illinois"
      />
      <HousingProps
        :building="'/public/images/Rectangle 15.png'"
        title="woodlandside"
        amount="$ 20. 000. 000"
        :profilePicture="'/public/images/Ellipse 6.png'"
        name="Robert Fox"
        description="Dr. San Jose, South Dakota"
      />
    </div>
  </div>
</template>

<script>
import HeadlineProps from './HeadlineProps.vue'
import HousingProps from './HousingProps.vue'

export default {
  name: 'FeatureHouse',
  components: { HeadlineProps, HousingProps }
}
</script>

<style scoped>
.feature-container-wrapper {
  margin-top: 7rem;
}

.feature {
  padding-top: 5rem;
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin-right: 46px;
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

.housing-props-container {
  display: flex;
  align-items: center;
  justify-content: space-between;
  flex-wrap: wrap;
  gap: 14px;
  padding-top: 40px;
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
@media (max-width: 1156px) {
  .housing-props-container {
    display: grid;
    gap: 50px;
    grid-template-columns: repeat(2, 1fr);
  }
}
</style>
