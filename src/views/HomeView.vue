<template>
    <div class="common-layout">
        <el-container>
            <el-header class="headers">Header</el-header>
            <el-container>
                <el-aside width="200px" class="aside">Aside</el-aside>
                <el-main class="main">Main</el-main>
            </el-container>

        </el-container>
    </div>
</template>

<script setup>
import { ref } from 'vue'
const name = ref('home')
console.log(name.value)
</script>

<style lang="scss" scoped>
$headers: 60px;
.common-layout {
  width: 100%;
  height: 100vh;
  background-color: #e5e5e5;
  .headers {
    height: $headers;
    background-color: #0091ff;
  }
  .aside {
    width: 200px;
    background-color: #07b39f;
  }
  .main {
    height: calc(100vh - #{$headers});
    background-color: #f5f5f5;
  }
  .footer {
    background-color: #4c4478;
  }
}
</style>
