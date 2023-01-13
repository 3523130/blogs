<template>  
  <headerView></headerView>
  <div class="container">
    <forFlow></forFlow>
    <sideBar></sideBar>
  </div>
  <dialogView></dialogView>
</template>

<script setup lang="ts">
import { ref } from 'vue'
import headerView from '@/components/header.vue';
import forFlow from './module/forFlow.vue';
import sideBar from './module/sideBar.vue';
import dialogView from '@/components/dialog.vue'
</script>

<style scoped lang="scss">
  .container{
    max-width: 1500px;
    height: 100%;
    margin: 0 auto;
    display: grid;
    grid-template-columns: 1fr 19vw;
    grid-template-rows: 1fr 1fr;
    grid-template-areas:
        "main right"
        "main right"
        "main right";
    height: 100vh;
  }
  @media screen and (max-width: 1366px){
    .container {
      display: grid;
      grid-template-columns: 1fr 280px;
    }
  }
  @media screen and (max-width: 768px){
    .container {
    grid-template-columns: 1fr;
    grid-template-rows: 1fr 1fr;
    grid-template-areas:
        "main main";
    }
  }
  

</style>
