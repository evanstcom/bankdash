<template>
  <div class="mobile-header">
    <div class="mobile-header__container">
      <img src="/burger.svg" alt="menu" />
      <h2 class="mobile-header__title">Setting</h2>
      <div><img class="foto" src="/foto.png" alt="" /></div>
    </div>
    <div class="input__container">
      <input class="input" type="text" placeholder="Search for something" />
      <img class="search__icon" src="/search.svg" alt="search" />
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.mobile-header {
  padding: 22px 25px;
  display: none;
  gap: 16px;
  flex-direction: column;
  background-color: #fff;
}
.mobile-header__container {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.mobile-header__title {
  font-size: 20px;
  color: #343c6a;
}
.input__container {
  position: relative;
}
.input {
  background-color: #f5f7fa;
  outline: none;
  width: 100%;
  height: 40px;
  border-radius: 30px;
  border: none;
  padding: 16px 10px 16px 46px;
  font-size: 15px;
  color: #343c6a;
}
.input::placeholder {
  color: #8ba3cb;
  font-size: 13px;
  padding-left: 0;
  letter-spacing: 0.4px;
}
.foto {
  width: 35px;
  height: 35px;
  border-radius: 50%;
  overflow: hidden;
}

.search__icon {
  position: absolute;
  width: 16px;
  left: 20px;
  top: 50%;
  transform: translateY(-50%);
}
@media screen and (max-width: 1024px) {
  .mobile-header {
    display: flex;
  }
}
</style>
