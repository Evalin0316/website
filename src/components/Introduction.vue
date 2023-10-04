<script setup>
import { ref } from 'vue'

defineProps({
  msg: String,
})

const count = ref(0)
</script>

<template>
<div class="p-24 m-auto font-semibold">
  <div class="text-2xl mb-4 text-black">我是Eva，目前有兩年多的前端工程師工作經驗</div>
  <div class="text-black">我很享受與人合作建構產品開發，<br>
  期望自己能不斷的透過解決問題的過程，提升自己的能力，提供用戶更良好的使用體驗。</div>
</div>
</template>

<style scoped lang="scss">
</style>
