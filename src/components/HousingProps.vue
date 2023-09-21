<template>
  <div class="housing-props-wrapper">
    <p>{{ title }}</p>
    <p>{{ amount }}</p>
    <div class="profile-content-wrapper">
      {{ profilePicture }}
      <div class="name-and-description">
        <p>{{ name }}</p>
        <p>{{ description }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HousingProps'
}
</script>

<style scoped>
.profile-content-wrapper {
  display: flex;
  align-items: center;
}
</style>
