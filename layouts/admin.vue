<template>
  <div class="admin-layout-wrap">
    <el-container :style="{height: '100%'}">
      <el-aside width="250px">
        <app-aside />
      </el-aside>
      <el-main>
        <nuxt />
      </el-main>
    </el-container>
  </div>
</template>

<script>
import AppAside from '@/components/admin/Aside';

export default {
  components: {
    AppAside,
  },
  computed: {
    error() {
      return this.$store.getters.error
    }
  },

  watch: {
    error(value) {
      this.$message.error(value.response.data.message);
    }
  }
}
</script>

<style lang="scss" scoped>
  .admin-layout-wrap {
    height: 100vh;
    width: 100%;
  }
</style>
