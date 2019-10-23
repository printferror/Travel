<template>
  <div>
    <div class="recommend-title">热销推荐</div>
    <ul>
      <li class="item border-bottom" v-for="item of recommendList" :key="item.index">
        <img class="item-img" :src="item.imgUrl"/>
        <div class="item-info">
          <p class="item-tile">{{item.title}}</p>
          <p class="item-desc">{{item.description}}</p>
          <button class="item-button">查看详情</button>
        </div>
        <p></p>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HomeRecommend',
  data () {
    return {
      recommendList: [{
        id: '0001',
        imgUrl: 'https://imgs.qunarzz.com/p/tts9/1901/19/ff4871ded7f05d02.jpg_110x110_aeced45b.jpg',
        title: '大连盛海海洋世界',
        description: '烂漫大连首站，浪漫的海洋主题乐园'
      },
      {
        id: '0002',
        imgUrl: 'https://imgs.qunarzz.com/p/tts9/1901/19/ff4871ded7f05d02.jpg_110x110_aeced45b.jpg',
        title: '大连盛海海洋世界',
        description: '烂漫大连首站，浪漫的海洋主题乐园'
      },
      {
        id: '0003',
        imgUrl: 'https://imgs.qunarzz.com/p/tts9/1901/19/ff4871ded7f05d02.jpg_110x110_aeced45b.jpg',
        title: '大连盛海海洋世界',
        description: '烂漫大连首站，浪漫的海洋主题乐园'
      },
      {
        id: '0004',
        imgUrl: 'https://imgs.qunarzz.com/p/tts9/1901/19/ff4871ded7f05d02.jpg_110x110_aeced45b.jpg',
        title: '大连盛海海洋世界',
        description: '烂漫大连首站，浪漫的海洋主题乐园'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
  @import '~styles/mixins.styl'
  .recommend-title
    margin-top: .8rem
    padding: 0.2rem 1rem
    line-height: 1.6rem
    background: #ccc
    text-indent: .2rem
  .item
    overflow: hidden
    display: flex
    height: 7rem
    .item-img
      height: 6.2rem
      width: 6.2rem
      margin: 0.4rem
    .item-info
      flex: 1
      margin: 0.4rem
      min-width: 0
      .item-tile
        line-height: 2rem
        font-size: 1.8rem
        ellipsis ()
      .item-desc
        line-height: 1.8rem
        color: #ccc
        ellipsis ()
      .item-button
        background: #ff9300
        padding: .15rem 1rem
        margin: .3rem .4rem
        border-radiu: 1rem
        color: white
        border: 0
</style>
