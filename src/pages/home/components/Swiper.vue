<template>
    <div class="wrapper">
        <swiper :options="swiperOption">
            <!-- slides -->
            <swiper-slide v-for="item of swiperList" :key="item.id">
                <img class="swiper-img" :src="item.imgUrl">
            </swiper-slide>    
            <!-- Optional controls -->
            <div class="swiper-pagination"  slot="pagination"></div>
        </swiper>
    </div>
</template>
<script>
    export default {
        name:'HomeSwiper',
        data (){
            return {
                swiperOption:{
                    pagination:'.swiper-pagination',
                    loop:true,
                    autoplay:3000,
                    autoplayDisableOnInteraction:false
                },
                swiperList:[
                    {
                        id:'0001',
                        imgUrl:'http://img1.qunarzz.com/piao/fusion/1807/66/e5a5cec881702f02.jpg_750x200_67bb5691.jpg'
                    }, {
                        id:'0002',
                        imgUrl:'http://img1.qunarzz.com/piao/fusion/1807/fa/800bd7f554abf302.jpg_750x200_9d809aad.jpg'
                    }
                ]
            }
        }
    }
</script>
<style lang="stylus" scoped>
    .wrapper >>> .swiper-pagination-bullet-active
        background :#fff
    .wrapper
        width:100%
        height:0
        overflow :hidden
        background :#eee
        padding-bottom :26.66%
        .swiper-img
            width:100%
</style>
