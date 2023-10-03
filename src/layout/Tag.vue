<template>
<div>
    <div v-for="(item,idx) in TagItem" :key="idx">
        <div class="tag">{{item}}</div>
    </div>
</div>
</template>

<script>
export default {
    props:['TagItem']
}
</script>

<style scoped lang="scss">
.tag{
    background:#F5DEB3;
    border-radius: 20px;
    margin: 0 10px;
}
</style>