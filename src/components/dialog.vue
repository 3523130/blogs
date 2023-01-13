<template>
    <div class="dialog">
      <div class="dialog_cont">
      </div>
    </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'
</script>

<style scoped>
.dialog{
  width: 100%;
  height: 100%;
  background-color: rgb(0, 0, 0, 0.5);
  position: fixed;
  left: 0px;
  top: 0px;
  z-index: 999;
  /* display: none; */
}
.dialog_cont{
  width: 515px;
  height: 300px;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%,-50%);
  background-color: #fff;
}
</style>
