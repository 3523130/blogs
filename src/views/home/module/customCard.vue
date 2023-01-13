<template>
    <div class="customCard" v-for="(item, index) in cardList" :key="item.id">
      <div class="custom_card_title">{{ item.title }}</div>
      <div class="custom_card_desc">{{ item.content }}</div>
    </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'
defineProps<{
  cardList: any
}>()
</script>

<style scoped>
.customCard{
  background-color: #fff;
  display: flex;
  flex-direction: column;
  animation: content-in .5s ease-in 0s;
  box-shadow: 0 2px 12px #0000001a;
  word-break: break-all;
}
@keyframes content-in {
  0% {
    transform: translateY(10rem);
    opacity: 0;
  }
  100% {
    transform: translateY(0);
    opacity: 1;
  }
}
.custom_card_title{
  padding: 20px 20px 8px;
  font-size: 14px;
  color: #2c2c2c;
  cursor: pointer;
}
.custom_card_title:hover{
  color: #1687fa;
}
.custom_card_desc{
  color: #8e8e8e;
  padding: 0 20px 8px;
  flex-grow: 1;
  font-size: 13px;
}
</style>
