<template>
  <div class="housing-props-wrapper">
    <div class="housing-image-container">
      <img class="building" :src="building" />
    </div>
    <p class="housing-title">{{ title }}</p>
    <p class="housing-amount">{{ amount }}</p>
    <div class="profile-content-wrapper">
      <img :src="profilePicture" />
      <div class="name-and-description">
        <p class="profile-name">{{ name }}</p>
        <p class="profile-description">{{ description }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HousingProps',
  props: ['title', 'amount', 'building', 'profilePicture', 'name', 'description']
}
</script>

<style scoped>
.housing-props-wrapper {
  min-width: 120px;
}

.housing-image-container {
  max-width: 450px;
  height: 250px;
  margin-bottom: 24px;
}
.building {
  object-fit: cover;
  width: 100%;
  height: 250px;
  border-radius: 23px;
}
.profile-content-wrapper {
  display: flex;
  align-items: flex-end;
}
.profile-description {
  color: var(--par-color);
  font-size: 0.8rem;
}
.name-and-description {
  margin: 24px 0 0 16px;
}
.housing-title {
  font-size: 1.2rem;
}
.housing-amount {
  font-size: 1rem;
  color: var(--par-color);
}
</style>
