<template>
 <el-row>
  <!-- 左边logo -->
  <el-col :span="4" class="logo">
   <div>logo</div>
  </el-col>
  <!-- 中间导航区域 -->
  <el-col :span="16">
   <el-menu
    :default-active="activeIndex2"
    class="menu"
    router
    mode="horizontal"
    @select="handleSelect"
    background-color="#545c64"
    text-color="#fff"
    active-text-color="#ffd04b">
    <el-menu-item index="1">处理中心</el-menu-item>
    <el-submenu index="2">
     <template slot="title">我的工作台</template>
     <el-menu-item index="2-1">选项1</el-menu-item>
     <el-menu-item index="2-2">选项2</el-menu-item>
     <el-menu-item index="2-3">选项3</el-menu-item>
    </el-submenu>
    <el-menu-item index="3"><a href="https://www.ele.me" rel="external nofollow" target="_blank">订单管理</a></el-menu-item>
   </el-menu>
  </el-col>
  <!-- 右边用户信息以及登陆注册 -->
  <el-button-group>
   <el-button type="danger" size="small" round >login</el-button>
   <el-button type="success" size="small" round >regin</el-button>
  </el-button-group>
 </el-row>
</template>
<script>
export default {
 // ...
}
</script>
<style scoped>
 
</style>