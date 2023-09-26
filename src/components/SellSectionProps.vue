<template>
  <div class="sell-section-container">
    <img class="picture-props" :src="picture" />
    <div class="content-container">
      <div class="profile-wrapper">
        <img class="small-profile-pix" :src="smallPix" />
        <p>{{ name }}</p>
      </div>
      <p class="title">{{ content }}</p>
      <div class="min-ago">
        <i class="las la-clock"></i>
        <p>{{ timeline }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'SellSectionProps',
  props: ['smallPix', 'content', 'name', 'picture', 'timeline']
}
</script>

<style>
.content-container .title {
  color: var(--head-color);
  font-size: 1rem;
  line-height: 22px;
  margin: 14px 0;
}

.min-ago {
  display: flex;
  align-items: center;
}
.sell-section-container {
  min-width: 330px;
  display: flex;
  gap: 32px;
}

.picture-props {
  border-radius: 12px;
  width: 40%;
  height: auto;
  object-fit: cover;
}
</style>
