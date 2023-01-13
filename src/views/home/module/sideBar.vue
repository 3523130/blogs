<template>
    <div class="sideBar">
      <div class="sidebar_categories">
        <div class="sidebar_postcategory">
          <h3 class="catListTitle">随笔分类</h3>
          <ul>
            <li>Vue(1)</li>
            <li>Node(1)</li>
            <li>踩坑(1)</li>
            <li>JavaScript(1)</li>
          </ul>
        </div>
      </div>
    </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'
</script>

<style scoped>
.sideBar{
  grid-area: right;
  background-color: #fff;
  margin-top: 35px;
}
@media screen and (max-width: 768px){
  .sideBar {
      display: none;
  }
}
@media screen and (max-width: 767px){
  .sideBar {
    display: none;
  }
}
@media screen and (max-width: 768px){
  .sideBar {
    grid-area: none;
  }
}
.catListTitle{
  color: #2c2c2c;
  font-size: 20px;
  margin-bottom: 16px;
  font-weight: 500;
}
.sidebar_postcategory{
  padding: 20px 20px 0;
}
.sidebar_postcategory ul li{
  padding: 8px;
  font-size: 16px;
  cursor: pointer;
}
</style>
