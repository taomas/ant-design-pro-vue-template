<script setup lang="ts">
import { useError } from './hooks/useError'

const { handleBack } = useError()
</script>

<template>
  <a-result status="404" title="404" sub-title="对不起，当前访问的页面不存在！">
    <template #extra>
      <a-button type="primary" @click="handleBack">
        返回首页
      </a-button>
    </template>
  </a-result>
</template>
