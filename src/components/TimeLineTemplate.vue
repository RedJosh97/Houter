<template>
  <div class="timeline-template-container">
    <div class="sample-image-container">
      <img class="sample-image" :src="sampleImage" />
    </div>
    <div class="content-container">
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
  min-width: 600px;
  height: 440px;
}

.sample-image {
  width: 90%;
  height: 320px;
  border-radius: 9px;
  object-fit: cover;
}

.content-container p {
  font-size: 0.9rem;
}
.content-container {
  background: #fff;
  margin: 0 auto;
  width: 450px;
  padding: 12px 32px;
  display: flex;
  border-radius: 16px;
  gap: 15px;
  flex-direction: column;
  transform: translateX(-6%) translateY(-60%);
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
