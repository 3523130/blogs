<template>
    <div class="forFlow">
      <div class="cards_list">
        <customCard></customCard>
      </div>
    </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'
import customCard from './customCard.vue';
</script>

<style scoped>
.forFlow{
  width: 1286px;
  background-color: #fff;
}
.cards_list{
  margin: 1rem 0;
  display: grid;
  grid-template-columns: repeat(3,1fr);
  grid-gap: 1rem;
}
</style>
