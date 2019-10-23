<template>
    <div class="header">
        <div class="header-left">
            <div class="iconfont back-icon">&#xe608;</div>
        </div>
        <div class="header-input">
            <span class="iconfont iconfont-ss">&#xe62a;</span>
            输入城市景点游玩主题
        </div>
        <div class="header-right">
            城市
            <span class="iconfont arrow-icon">&#xe64a;</span>
        </div>
    </div>
</template>

<script>
export default {
  name: 'Home'
}
</script>

<style lang="stylus" scoped>
    @import '~styles/varibles.styl'
    .header
        display flex
        line-height: 3.44rem
        background: $bgColor
        .header-left
            width: 2.56rem
            float: left
            .back-icon
                text-align:center;
                font-size: 1.6rem
        .header-input
            flex: 1
            height:2.4rem;
            line-height: 2.56rem
            margin-top: .48rem
            margin-left: .8rem
            padding-left:.5rem
            background: #fff
            border-radius: .4rem
            color: #ccc
            .iconfont-ss
                color:black
        .header-right
            color:white
            width: 4.96rem
            float: right
            text-align: center
            .arrow-icon
                margin-left: -.15rem
                font-size: .2rem
        .iconfont
            color:white
</style>
