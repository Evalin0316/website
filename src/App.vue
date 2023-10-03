<script setup>
import introduction from './components/Introduction.vue'
import project from './components/Project.vue'
import pagefooter from './layout/PageFooter.vue'
import pageheader from './layout/PageHeader.vue'
</script>

<template>
 <div>
  <pageheader/>
    <introduction msg="Vite + Vue" />
    <project/>
  <pagefooter/>
</div>
</template>

<style scoped>
</style>
