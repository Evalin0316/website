<template>
<div class="tag_container flex flex-wrap">
    <div v-for="(item,idx) in TagItem" :key="idx">
        <div class="tag_container__tag">{{item}}</div>
    </div>
</div>
</template>

<script>
export default {
    props:['TagItem']
}
</script>

<style scoped lang="scss">
.tag_container{
    display: flex;
    flex-wrap: wrap;
    &__tag{
        background:#F5DEB3;
        border-radius: 4px;
        margin: 0 10px;
        padding: 0 10px;
    }
}
</style>