<template>
  <el-button type="primary" plain>
    <NuxtLink to="/" class="n-link-base"> Home </NuxtLink>
  </el-button>
  <el-button type="primary" plain>
    <NuxtLink to="/about"> About </NuxtLink>
  </el-button>
  <NuxtLink to="/about"> About </NuxtLink>
  <el-card shadow="never">
    <p style="text-align: center">
      Current route: <code>{{ route.path }}</code>
    </p>
  </el-card>
</template>
<script setup lang="ts">
const route = useRoute();
</script>
