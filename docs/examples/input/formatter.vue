<template>
  <el-input
    v-model="input"
    style="width: 240px"
    placeholder="Please input"
    :formatter="(value) => `实打实的 ${value}`"
    :parser="(value) => value.replace(/\$\s?|(,*)/g, '')"
  />
</template>

<script lang="ts" setup>
import { ref } from 'vue'
const input = ref('')
</script>
