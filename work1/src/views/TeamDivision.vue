<template>
    <div class="teamwork">
        <h2>项目分工</h2>
        <ul>
            <li v-for="(item,index) in team" :key="index">
                <span>{{item.name}}</span>
                <span>{{item.task}}</span>
            </li>
        </ul>
        </div>
</template>
<script setup lang="ts">
import {reactive} from 'vue'
const team=reactive([
    {name:"黄晶",task:"用户模块"},
    {name:"杨雅琪",task:"社团管理员模块"},
    {name:"鲁颖",task:"管理员模块"},
])

</script>

<style scoped lang="scss"> 
.teamwork {
  max-width: 800px;
  margin: 2rem auto;
  padding: 2rem;
  h2 {
    color: #2c3e50;
    font-size: 1.8rem;
    margin-bottom: 1.5rem;
    padding-left: 1rem;
  }
  ul {
    list-style: none;
    padding: 0;
    li {
      background: white;
      color:black;
      margin: 1rem 0;
      padding: 1.5rem;
      border-radius: 8px;
      box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
      display: flex;
      align-items: center;
      span {
        font-weight: 600;
        color: black;
        margin-right: 0.8rem;
        min-width: 80px;
      }
    }
  }
}
</style>