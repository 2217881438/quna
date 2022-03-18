<template>
    <div>
        <city-header></city-header>
        <city-search></city-search>
    </div>
</template>

<script>
import cityHeader from './components/Header'
import citySearch from './components/Search'
    export default {
        name: "cityCity",
        components: {
            cityHeader,
            citySearch
        }
    }
</script>

<style lang="less" scoped>

</style>