<template>
  <el-menu
    :style="{height: '100%'}"
    :default-active="$route.path"
    router
  >
    <el-menu-item index="/admin">
      <i class="el-icon-menu"></i>
      <span>Analytics</span>
    </el-menu-item>
    <el-menu-item index="/admin/create">
      <i class="el-icon-edit-outline"></i>
      <span>Create</span>
    </el-menu-item>
    <el-menu-item index="/admin/list">
      <i class="el-icon-tickets"></i>
      <span>Posts</span>
    </el-menu-item>
    <el-menu-item index="/admin/user">
      <i class="el-icon-service"></i>
      <span>Users</span>
    </el-menu-item>
    <el-menu-item index="/admin/logout">
      <i class="el-icon-setting"></i>
      <span>Logout</span>
    </el-menu-item>
  </el-menu>
</template>
