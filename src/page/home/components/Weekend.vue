<template>
  <div>
    <div class="recommend-title">周末去哪儿</div>
    <ul>
      <li class="item border-bottom" v-for="item of recommendList" :key="item.index">
        <div class="item-img-wrapper">
          <img class="item-img" :src="item.imgUrl"/>
        </div>
        <div class="item-info">
          <p class="item-tile">{{item.title}}</p>
          <p class="item-desc">{{item.description}}</p>
        </div>
        <p></p>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'WeekendIcons',
  data () {
    return {
      recommendList: [{
        id: '0001',
        imgUrl: 'https://imgs.qunarzz.com/p/tts4/1903/63/9606746325730902.jpg_750x440_0a7058dd.jpg',
        title: '大连盛海海洋世界',
        description: '烂漫大连首站，浪漫的海洋主题乐园'
      },
      {
        id: '0002',
        imgUrl: 'https://imgs.qunarzz.com/p/tts4/1903/63/9606746325730902.jpg_750x440_0a7058dd.jpg',
        title: '大连盛海海洋世界',
        description: '烂漫大连首站，浪漫的海洋主题乐园'
      },
      {
        id: '0003',
        imgUrl: 'https://imgs.qunarzz.com/p/tts4/1903/63/9606746325730902.jpg_750x440_0a7058dd.jpg',
        title: '大连盛海海洋世界',
        description: '烂漫大连首站，浪漫的海洋主题乐园'
      },
      {
        id: '0004',
        imgUrl: 'https://imgs.qunarzz.com/p/tts4/1903/63/9606746325730902.jpg_750x440_0a7058dd.jpg',
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
  .item-img
    width: 100%
  .item-img-wrapper
    height: 0
    overflow: hidden
    width: 100%
    padding-bottom: 36%
  .item-info
    flex: 1
    margin: 0.2rem 0 1rem 0
    min-width: 0
    .item-tile
      line-height: 2rem
      font-size: 1.8rem
      ellipsis ()
    .item-desc
      line-height: 1.8rem
      color: #ccc
      ellipsis ()
</style>
