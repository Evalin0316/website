<script setup>
import { ref } from 'vue'

defineProps({
  msg: String,
})

const count = ref(0)
</script>

<template>
<div class="">
  嗨，我是Eva，目前有兩年多的前端工程師的工作經驗。我喜歡與人合作...
</div>
</template>

<style scoped lang="scss">
.read-the-docs {
  color: #888;
}
</style>
