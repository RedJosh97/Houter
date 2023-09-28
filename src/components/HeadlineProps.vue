<template>
  <div class="headline-props">
    <p class="subtitle">{{ subTitle }}</p>
    <p class="title">{{ title }}</p>
    <slot name="displayOther"></slot>
  </div>
</template>

<script>
export default {
  name: 'HeadlineProps',
  props: ['subTitle', 'title']
}
</script>

<style scoped>
.subtitle::before {
  content: '';
  position: absolute;
  top: 7px;
  left: 51px;
  width: 40px;
  height: 3px;
  background: var(--sub-color);
  border-radius: 14px;
}
.title {
  color: var(--head-color);
  font-size: 2rem;
  font-weight: 600;
  margin-bottom: 1.5rem;
}
.subtitle {
  color: var(--sub-color);
  font-size: 0.8rem;
}
</style>
