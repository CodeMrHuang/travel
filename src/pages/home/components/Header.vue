<template>
    <div class="header">
        <div class="header-left">
            <div class="iconfont icon-fanhui"></div>
        </div>
        <div class="header-input">
            <span class="iconfont icon-sousuo"></span>
            输入城市/景点/游玩主题
        </div>
        <div class="header-right">
            城市
            <span class="iconfont icon-jiantou"></span>
        </div>
    </div>
</template>
<script>
    export default {
        name:'HomeHeader'
    }
</script>
<style lang="stylus" scoped>
    @import '~styles/varibles.styl' 
    .header
        display:flex
        height: .86rem
        line-height :.86rem
        background :$bgColor
        color :#fff
        .header-left
            width: .64rem
            float: left
            .icon-fanhui
                text-align :center
                font-size :.4rem
        .header-input
            flex:1
            height :.62rem
            margin-top :.12rem
            margin-left :.2rem
            background :#fff
            border-radius :.1rem
            color :#ccc
            line-height .62rem
            padding-left :.2rem
        .header-right
            width: 1.24rem
            float: left
            text-align:center 
            .icon-jiantou
                font-size :.24rem
                margin-left :-.04rem
</style>
