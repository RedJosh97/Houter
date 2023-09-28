<template>
  <div class="sub-section">
    <div class="sub-container">
      <img class="float-1 small-float-box" src="/public/images/Rectangle 15-3.png" />
      <img class="float-2 tiny-float-box" src="/public/images/Ellipse 6-3.png" />
      <img class="float-3 tiny-float-box" src="/public/images/Ellipse 6.png" />
      <img class="float-4 small-float-box" src="/public/images/Rectangle 17.png" />
      <img class="float-5 tiny-float-box" src="/public/images/Rectangle 15-1.png" />
      <img class="float-6 tiny-float-box" src="/public/images/Ellipse 6-2.png" />
      <img class="float-7 tiny-float-box" src="/public/images/Ellipse 6-3.png" />
      <img class="float-8 small-float-box" src="/public/images/Rectangle 15.png" />
      <div class="sub-wrapper">
        <p>Subscribe For More Info and update from Hounter</p>
        <div class="input-field">
          <div class="input-wrapper">
            <i class="las la-envelope-open"></i>
            <input type="text" placeholder="add your email here" v-model="textInput" />
          </div>
          <button class="contact-box-btn">Subscribe now</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'SubscribeLayout'
}
</script>

<style>
.sub-section {
  margin-top: 4rem;
  padding: 0 7rem;
}

.sub-container {
  background: linear-gradient(40deg, #8a82e8, #8cd2f2, #8a82e8);
  width: 100%;
  height: 312px;
  border-radius: 45px;
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
  position: relative;
}
.sub-wrapper p {
  color: var(--head-color);
  font-size: 32px;
  font-weight: 600;
}
.sub-wrapper {
  text-align: center;
  max-width: 496px;
  display: flex;
  flex-direction: column;
  gap: 47px;
}

.input-field {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 12px;
  background: #fff;
  margin: 0 1rem;
  border-radius: 32px;
  padding: 4px 4px 4px 24px;
  box-shadow: 0px 9px 32px 0px rgba(89, 92, 219, 0.05);
}
.input-wrapper {
  display: flex;
  gap: 16px;
  align-items: center;
}
.input-field input {
  border: none;
  padding: 4px;
}

.small-float-box {
  width: 81px;
  height: 81px;
  object-fit: cover;
  border-radius: 34px;
  border: 1.5px solid #fff;
}
.tiny-float-box {
  width: 36px;
  height: 36px;
  border-radius: 50px;
  object-fit: cover;
  border: 1.5px solid #fff;
}

.sub-container .float-1 {
  position: absolute;
  top: 50px;
  left: 40px;
}
.sub-container .float-2 {
  position: absolute;
  top: 180px;
  left: 60px;
}
.sub-container .float-3 {
  position: absolute;
  top: 71px;
  left: 190px;
}

.sub-container .float-4 {
  position: absolute;
  width: 50px;
  height: 50px;
  bottom: 60px;
  left: 180px;
}

.sub-container .float-5 {
  position: absolute;
  top: 120px;
  right: 70px;
  width: 27px;
  height: 27px;
}
.sub-container .float-6 {
  position: absolute;
  top: 219px;
  right: 60px;
}
.sub-container .float-7 {
  position: absolute;
  width: 32px;
  height: 32px;
  top: 181px;
  right: 190px;
}
.sub-container .float-8 {
  position: absolute;
  top: 31px;
  right: 140px;
  width: 70px;
  height: 70px;
}
</style>
