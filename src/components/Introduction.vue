<script setup>
import { ref } from 'vue'

defineProps({
  msg: String,
})

const count = ref(0)
</script>

<template>
<div>
  嗨，我是Eva，目前有兩年前端工程師的工作經驗。
</div>
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>
