<template>  
  <headerView></headerView>
  <div class="container">
    <forFlow></forFlow>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'
import headerView from '@/components/header.vue';
import forFlow from './module/forFlow.vue';
</script>

<style scoped lang="scss">
  .container{
    width: 1586px;
    height: 100%;
    margin: 0 auto;
  }
</style>
