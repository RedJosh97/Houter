<template>
  <div class="hero-section">
    <div class="hero-left-section">
      <h1>Find the place to live <span>your dreams</span> easily here</h1>
      <p>
        Everything you need about finding your place to live will be here, where it will be easier
        for you
      </p>
      <div class="search-box">
        <div>
          <i class="las la-map-marker"></i>
          <input type="text" placeholder="Search for the location you want!" />
        </div>
        <button class="search-box-btn">search <i class="las la-angle-right"></i></button>
      </div>

      <div class="partnership">
        <p>Our partnership</p>
        <div>
          <img src="/public/images/Frame 9.png" alt="" />
        </div>
      </div>
    </div>
    <div class="hero-right-section">
      <img src="/public/images/image6.png" alt="picture-frame" />
    </div>
  </div>
</template>

<script>
export default {
  name: 'NavBar.vue'
}
</script>

<style scoped>
.hero-section {
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 104px;
}
.partnership p {
  font-weight: 300;
  color: var(--par-color);
}

.hero-left-section {
  display: flex;
  justify-content: space-between;
  flex-direction: column;
  gap: 24px;
  margin-top: 20px;
  max-width: 496px;
  width: 40%;
}

.hero-left-section h1 {
  font-weight: 900;
  font-size: 2.5rem;
}

.hero-left-section span {
  font-weight: 900;
  font-size: 2.5rem;
  color: #fff;
  text-shadow: 0 0 4px #1b1c57;
}

.la-map-marker {
  color: orange;
}

.hero-left-section p {
  line-height: 28px;
}
.hero-left-section input {
  padding: 4px 4px 4px 24px;
  border-radius: 32px;
}
.search-box {
  display: flex;
  justify-content: space-between;
  align-items: center;
  border-radius: 32px;
  border: 1px solid #e0e3eb;
  padding: 4px 4px 4px 24px;
}
.search-box input {
  height: 22px;
  outline: none;
  border: none;
}
.search-box-btn {
  padding: 12px 16px;
  background: var(--deep-color);
  color: #fff;
  border-radius: 32px;
  border: none;
}
.hero-right-section img {
  width: 50%;
  height: 90vh;
  object-fit: cover;
  border-radius: 0px 0px 0px 80px;
  position: absolute;
  top: 0;
  right: 0;
  z-index: -10;
}
</style>
