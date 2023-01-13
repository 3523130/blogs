<template>
    <div class="forFlow">
      <div class="cards_list">
        <customCard :cardList="cardList"></customCard>
      </div>
    </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'
import customCard from './customCard.vue';

const cardList = [
  {id:1,title:'Vue 配置打包文件引入带上时间戳',content:'摘要： 撒大苏打飒飒发呢开萨兰兰德里但是考虑到昂克赛拉你打顺马上屏幕撒泼没打的方式开发破口'},
  {id:1,title:'Vue 配置打包文件引入带上时间戳',content:'摘要： 撒大苏打飒飒发呢开萨兰兰德里但是考虑到昂克赛拉你打顺马上屏幕撒泼没打的方式开发破口'},
  {id:1,title:'Vue 配置打包文件引入带上时间戳',content:'摘要： 撒大苏打飒飒发呢开萨兰兰德里但是考虑到昂克赛拉你打顺马上屏幕撒泼没打的方式开发破口'},
  {id:1,title:'Vue 配置打包文件引入带上时间戳',content:'摘要： 撒大苏打飒飒发呢开萨兰兰德里但是考虑到昂克赛拉你打顺马上屏幕撒泼没打的方式开发破口'},
  {id:1,title:'Vue 配置打包文件引入带上时间戳',content:'摘要： 撒大苏打飒飒发呢开萨兰兰德里但是考虑到昂克赛拉你打顺马上屏幕撒泼没打的方式开发破口'},
  {id:1,title:'Vue 配置打包文件引入带上时间戳',content:'摘要： 撒大苏打飒飒发呢开萨兰兰德里但是考虑到昂克赛拉你打顺马上屏幕撒泼没打的方式开发破口'},
  {id:1,title:'Vue 配置打包文件引入带上时间戳',content:'摘要： 撒大苏打飒飒发呢开萨兰兰德里但是考虑到昂克赛拉你打顺马上屏幕撒泼没打的方式开发破口'},
  {id:1,title:'Vue 配置打包文件引入带上时间戳',content:'摘要： 撒大苏打飒飒发呢开萨兰兰德里但是考虑到昂克赛拉你打顺马上屏幕撒泼没打的方式开发破口'},
  {id:1,title:'Vue 配置打包文件引入带上时间戳',content:'摘要： 撒大苏打飒飒发呢开萨兰兰德里但是考虑到昂克赛拉你打顺马上屏幕撒泼没打的方式开发破口'},
  {id:1,title:'Vue 配置打包文件引入带上时间戳',content:'摘要： 撒大苏打飒飒发呢开萨兰兰德里但是考虑到昂克赛拉你打顺马上屏幕撒泼没打的方式开发破口'},
  {id:1,title:'Vue 配置打包文件引入带上时间戳',content:'摘要： 撒大苏打飒飒发呢开萨兰兰德里但是考虑到昂克赛拉你打顺马上屏幕撒泼没打的方式开发破口'},
  {id:1,title:'Vue 配置打包文件引入带上时间戳',content:'摘要： 撒大苏打飒飒发呢开萨兰兰德里但是考虑到昂克赛拉你打顺马上屏幕撒泼没打的方式开发破口'},
  {id:1,title:'Vue 配置打包文件引入带上时间戳',content:'摘要： 撒大苏打飒飒发呢开萨兰兰德里但是考虑到昂克赛拉你打顺马上屏幕撒泼没打的方式开发破口'},
  {id:1,title:'Vue 配置打包文件引入带上时间戳',content:'摘要： 撒大苏打飒飒发呢开萨兰兰德里但是考虑到昂克赛拉你打顺马上屏幕撒泼没打的方式开发破口'},
  {id:1,title:'Vue 配置打包文件引入带上时间戳',content:'摘要： 撒大苏打飒飒发呢开萨兰兰德里但是考虑到昂克赛拉你打顺马上屏幕撒泼没打的方式开发破口'},
  {id:1,title:'Vue 配置打包文件引入带上时间戳',content:'摘要： 撒大苏打飒飒发呢开萨兰兰德里但是考虑到昂克赛拉你打顺马上屏幕撒泼没打的方式开发破口'},
]
</script>

<style scoped>
.forFlow{
  padding: 20px;
  display: grid;
  grid-template-rows: 1fr;
  grid-template-columns: 1fr;
  grid-area: main;
}
@media screen and (max-width: 768px){
  .forFlow {
    margin-top: 0;
    grid-area: auto;
    height: 100vh;
    padding: 10px;
  }
}

.cards_list{
  margin: 1rem 0;
  display: grid;
  grid-template-columns: repeat(3,1fr);
  grid-gap: 1rem;
  overflow-x: hidden;
  overflow-y: auto;
  padding-bottom: 20px;
}
@media screen and (max-width: 1175px){
  .cards_list {
    grid-template-columns: repeat(2,1fr);
  }
}
@media screen and (max-width: 908px){
  .cards_list {
    grid-template-columns: 1fr;
    grid-template-rows: auto;
  }
}
.cards_list::-webkit-scrollbar {
    width: 7px;
    height: 13px;
}
.cards_list::-webkit-scrollbar-thumb {
  background-color: #dedede;
}
.cards_list::-webkit-scrollbar-track {
  background-color: #f0f0f0;
  opacity: .15;
}
</style>
