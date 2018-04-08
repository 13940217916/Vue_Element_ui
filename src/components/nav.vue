<template>
  <div class="nav">
    <h5>Element ui</h5>
    <el-menu
      default-active="1"
      class="el-menu-vertical-demo"
      @open="handleOpen"
      @close="handleClose"
      text-color="#545c64"
      active-text-color="#ffd04b">
      <el-menu-item index="1">
        <span slot="title">学生信息</span>
      </el-menu-item>
      <el-menu-item index="2">
        <span slot="title">新生信息录入</span>
      </el-menu-item>
      <el-menu-item index="3">
        <span slot="title">学生信息</span>
      </el-menu-item>
    </el-menu>
  </div>
</template>

<script>
    export default {
      name: "",
      methods:{
        handleOpen(key, keyPath) {
          console.log(key, keyPath);
        },
        handleClose(key, keyPath) {
          console.log(key, keyPath);
        },
      }
    }
</script>

<style scoped>

</style>
