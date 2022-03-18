<template>
    <div class="search">
        <input type="text" class="search-input" placeholder="输入城市名或拼音">
    </div>
</template>

<script>
    export default {
        name: "citySearch"
    }
</script>

<style lang="less" scoped>
@import "./../../../assets/styles/varibles.less";
.search{
    height: .72rem;
    padding: 0 .1rem;
    background: @bdColor;
    .search-input{
        box-sizing: border-box;
        width: 100%;
        height:.62rem;
        padding: 0 .1rem;
        line-height: .62rem;
        text-align: center;
        border-radius: .06rem;
        color: #666;
    }
}
</style>