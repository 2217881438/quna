<template>
    <div class="wrapper">
        <swiper ref="mySwiper" :options="swiperOptions" v-if="showSwiper">
            <swiper-slide v-for="item of list" :key="item.id">
                <img class="swiper-img" :src="item.imgUrl" />
            </swiper-slide>
            <div class="swiper-pagination" slot="pagination"></div>
        </swiper>
    </div>
</template>

<script>
    export default {
        name:"HomeSwiper",
        props:{
            list: Array
        },
        data () {
            return{
                swiperOptions:{
                    loop:true,
                    pagination: ".swiper-pagination"
                },
            }
        },
        computed: {
            showSwiper () {
                return this.list.length
            }
        }
    }
</script>

<style lang="less" scoped>
    .wrapper{
        overflow: hidden;
        width: 7.48rem;
        height: 0;
        padding-bottom: 2.3rem;
        background: #eee;
        .swiper-img{
            width: 7.48rem;
            height: 2.3rem;
        }
    }
    
</style>