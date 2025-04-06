<template>
   <div class="intro">
    <h2>系统简介</h2>
    <p>{{ where }}</p>
    <h2>系统功能介绍</h2>
    <p>{{ work }}</p>
   </div>

</template>
<script setup lang="ts">
import {ref} from 'vue'
const where=ref("本系统是一个社团管理系统，主要用于社团的日常管理和信息发布。")
const work=ref("本系统主要包括社团信息管理、社团活动管理、社团成员管理、社团公告发布等功能。")

</script>

<style scoped lang="scss"> 
.intro {
  max-width: 800px;
  margin: 2rem auto;
  padding: 2rem;
  background: #f8f9fa;
  border-radius: 12px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  h2 {
    color: #2c3e50;
    font-size: 1.8rem;
    margin-bottom: 1.5rem;
    border-bottom: 2px solid #3498db;
    padding-bottom: 0.5rem;
  }
  p {
    font-size: 1.1rem;
    line-height: 1.6;
    color: #34495e;
    margin: 1rem 0;
    padding: 1rem;
    background: white;
    border-radius: 8px;
  }
}
</style>