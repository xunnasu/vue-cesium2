<template>
  <div class="v-page home-page flex-grid flex-col">
    首页
    <el-button type="primary" @click="handleClick">弹窗</el-button>
  </div>
</template>

<script setup>
import { ref } from 'vue';
import { ElMessageBox } from 'element-plus';

function handleClick() {
  ElMessageBox.confirm('Are you sure to close this dialog?')
    .then(() => {})
    .catch(() => {
      // catch error
    });
}
</script>

<style lang="scss" scoped></style>
