<template>
  <div>
    <p class="subtitle">{{ subTitle }}</p>
    <p class="title">{{ title }}</p>
  </div>
</template>

<script>
export default {
  name: 'HeadlineProps',
  props: ['subTitle', 'title']
}
</script>

<style scoped>
.title {
  color: var(--head-color);
  font-size: 2rem;
  font-weight: 600;
}
.subtitle {
  color: var(--sub-color);
  font-size: 0.8rem;
}
</style>
