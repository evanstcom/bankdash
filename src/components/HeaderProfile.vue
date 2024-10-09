<template>
  <MobileHeader />
  <header class="header">
    <h2 class="header__title">Setting</h2>
    <div class="header__setiing">
      <div class="input__container">
        <input class="input" type="text" placeholder="Search for something" />
        <img class="search__icon" src="/search.svg" alt="search" />
      </div>
      <div class="item-box">
        <img class="item-box__image" src="/settings_1.svg" alt="settings" />
      </div>
      <div class="item-box"><img src="/notification_1.svg" alt="notification" /></div>
      <div class="item-foto"><img src="/foto.png" alt="fot" /></div>
    </div>
  </header>
</template>

<script setup>
import MobileHeader from './MobileHeader.vue'
</script>

<style scoped>
header {
  width: 100%;
  min-height: 100px;
  background-color: #fff;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0 40px;
  border-bottom: 1px solid #e6eff5;
}
.header__title {
  color: #343c6a;
  font-size: 28px;
  font-weight: 600;
}
.header__setiing {
  display: flex;
  align-items: center;
  gap: 30px;
}

.input__container {
  position: relative;
}

.input {
  background-color: #f5f7fa;
  outline: none;
  width: 255px;
  height: 50px;
  border-radius: 30px;
  border: none;
  padding: 16px 10px 16px 60px;
  font-size: 15px;
  color: #343c6a;
}
.input::placeholder {
  color: #8ba3cb;
}

.search__icon {
  position: absolute;
  width: 20px;
  left: 20px;
  top: 50%;
  transform: translateY(-50%);
}

.item-box {
  width: 50px;
  height: 50px;
  border-radius: 50%;
  background-color: #f5f7fa;
  display: flex;
  align-items: center;
  justify-content: center;
}

.item-box__image {
  width: 25px;
}

.item-foto {
  width: 60px;
  height: 60px;
  border-radius: 50%;
  overflow: hidden;
  margin-left: 8px;
}
@media screen and (max-width: 1024px) {
  .header {
    display: none;
  }
}
</style>
