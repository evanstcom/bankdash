<template>
  <div class="navigation">
    <div class="logo__container">
      <a href=""><img class="logo__image" src="/Logo.svg" alt="Logo" /></a>
    </div>
    <div class="menu">
      <MenuItem v-for="item in menu" :key="item.name" :item="item" />
    </div>
  </div>
</template>

<script setup>
import MenuItem from './MenuItem.vue'
const menu = [
  {
    name: 'Dashboard',
    path: '/',
    img: '/1.svg'
  },
  {
    name: 'Transactions',
    path: '/',
    img: '/2.svg'
  },
  {
    name: 'Accounts',
    path: '/',
    img: '/3.svg'
  },
  {
    name: 'Investments',
    path: '/',
    img: '/4.svg'
  },
  {
    name: 'Credit Cards',
    path: '/',
    img: '/5.svg'
  },
  {
    name: 'Loans',
    path: '/',
    img: '/6.svg'
  },
  {
    name: 'Services',
    path: '/',
    img: '/7.svg'
  },
  {
    name: 'My Privileges',
    path: '/',
    img: '/8.svg'
  },
  {
    name: 'Setting',
    path: '/',
    img: '/9.svg',
    active: true
  }
]
</script>

<style scoped>
.navigation {
  display: flex;
  flex-direction: column;
  width: 300px;
  border-right: 1px solid #e6eff5;
  height: 100vh;
  background-color: #fff;
}
.logo__container {
  display: flex;
  align-items: center;
  height: 100px;
  padding-left: 44px;
}

.logo__image {
  width: 183px;
}

.menu {
  display: flex;
  flex-direction: column;
  gap: 36px;
  padding: 30px 0 0 44px;
}

@media screen and (max-width: 1024px) {
  .navigation {
    display: none;
  }
}
</style>
