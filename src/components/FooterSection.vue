<template>
  <div class="footer-section">
    <div class="left-side-wrapper">
      <div class="logo">
        <img src="/public/images/logo.svg" />
        <p class="head-text">hounter</p>
      </div>
      <p>
        We provide information about properties such as houses, villas and apartments to help people
        find their dream home
      </p>
      <div class="social-icon">
        <i class="lab la-facebook-f"></i>
        <i class="lab la-twitter"></i>
        <i class="lab la-instagram"></i>
      </div>
    </div>
    <div class="right-side-wrapper">
      <img class="clipper" src="/public/images/Vector (4).png" />
      <img class="clipper2" src="/public/images/Vector (5).png" />
      <div class="item-wrapper">
        <p class="head-text">Property</p>
        <p>House</p>
        <p>Apartment</p>
        <p>Villa</p>
      </div>
      <div class="item-wrapper">
        <p class="head-text">Article</p>
        <p>New Article</p>
        <p>Popular Article</p>
        <p>Most Read</p>
        <p>Tip & Tricks</p>
      </div>
      <div class="item-wrapper">
        <p class="head-text">Contact</p>
        <p>459 Royal ln, Mesa, New Jersey 45463</p>
        <p>(671)-555-109</p>
        <p>info@hounter.com</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'FooterSection'
}
</script>

<style scoped>
.footer-section {
  margin-top: 4rem;
  display: flex;
  color: var(--par-color);
  justify-content: space-between;
  font-size: 0.9rem;
  line-height: 24px;
  font-size: 12.5px;
  gap: 32px;
  position: relative;
  padding: 0 7rem;
}

.head-text {
  color: var(--head-color);
  font-weight: 700;
}
.logo {
  display: flex;
  align-items: center;
  gap: 12px;
}
.social-icon {
  display: flex;
  gap: 12px;
  align-items: center;
  color: var(--head-color);
  border-radius: 50px;
  font-size: 34px;
}

.clipper2 {
  position: absolute;
  top: -280px;
  right: -120px;
}
.clipper {
  position: absolute;
  top: -200px;
  right: -40px;
  width: 350px;
  transform: rotate(270deg);
}

.left-side-wrapper {
  max-width: 330px;
  display: flex;
  /* align-items: flex-start; */
  justify-content: space-evenly;
  flex-direction: column;
  gap: 23px;
}
.right-side-wrapper {
  display: flex;
  flex-wrap: wrap;
  gap: 30px;
  line-height: 30px;
  justify-content: end;
}
</style>
