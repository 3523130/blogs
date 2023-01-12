<template>
    <div class="customCard">
      <div class="custom_card_title">这里是title</div>
      <div class="custom_card_desc">这里是内容阿</div>
    </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'
</script>

<style scoped>
.custom_card_title{
  padding: 20px 20px 8px;
  font-size: 14px;
  color: #2c2c2c;
}
.custom_card_desc{
  color: #8e8e8e;
  padding: 0 20px 8px;
  flex-grow: 1;
  font-size: 13px;
}
</style>
