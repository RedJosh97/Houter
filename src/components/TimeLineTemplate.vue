<template>
  <div class="timeline-template-container">
    <img class="sample-image" :src="sampleImage" />
    <div class="content-container">
      <div class="text-content-wrapper"></div>
      <p>{{ title }}</p>
      <p>{{ content }}</p>
      <div class="profile-content-wrapper">
        <div class="name-and-description">
          <img class="pro-img" :src="profileImage" />
          <p>{{ profileName }}</p>
          <p>{{ profileDescription }}</p>
        </div>
        <div class="rating">
          <i class="las la-star"></i>
          <p>{{ rating }}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'TimeLineTemplate',
  props: [
    'profileDescription',
    'profileName',
    'profileImage',
    'content',
    'title',
    'rating',
    'sampleImage'
  ]
}
</script>

<style scoped>
.timeline-template-container {
  max-width: 740px;
  position: relative;
}

.sample-image {
  width: 100%;
  height: 420px;
  border-radius: 9px;
  object-fit: cover;
}

.content-container {
  background: #fff;
  margin: 0 auto;
  max-width: 612px;
  min-width: 110px;
  padding: 9px 32px;
  display: flex;
  border-radius: 16px;
  gap: 24px;
  flex-direction: column;
  transform: translateY(-60%);
}
.pro-img {
  margin-right: 16px;
}
.profile-content-wrapper {
  display: flex;
  max-width: 612px;
  justify-content: space-between;
  align-items: center;
}
.name-and-description {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.la-star {
  color: #f59e0b;
}
.rating {
  display: flex;
  align-items: center;
  gap: 16px;
}
</style>
