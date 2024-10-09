<template>
  <div class="item">
    <div :class="item.active ? 'border' : ''">
      <img class="item__image" :src="item.img" alt="" />
    </div>
    <span :class="item.active ? 'item__name_active item__name' : 'item__name '">{{
      item.name
    }}</span>
  </div>
</template>

<script setup>
defineProps({
  item: {
    type: Object
  }
})
</script>

<style scoped>
.item {
  display: flex;
  align-items: center;
  gap: 26px;
  cursor: pointer;
  position: relative;
}

.item__image {
  width: 25px;
  height: 25px;
}

.item__name {
  font-size: 18px;
  font-weight: medium;
  color: #b1b1b1;
  transition: color 0.3s ease-in-out;
}
.item__name_active {
  color: #1814f3;
}

.item:hover .item__name {
  color: #1814f3;
}

.item:hover .item__name {
  color: #1814f3;
}

.border::before {
  content: '';
  display: block;
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  left: -50px;
  height: 60px;
  border-left: 12px solid #1814f3;
  border-radius: 10px;
}
</style>
