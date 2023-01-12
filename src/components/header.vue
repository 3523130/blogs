<template>
  <div class="header">
    <a href="javascript:;" class="">首页</a>
    <p>风</p>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'
</script>

<style scoped lang="scss">
.header{
  background-color: #fff;
  width: 100%;
  height: 45px;
  display: flex;
  justify-content: space-between;
  line-height: 45px;
  box-sizing: border-box;
  padding: 0 40px;
  font-size: 20px;

  a{
    color: #000;
  }
}
</style>
