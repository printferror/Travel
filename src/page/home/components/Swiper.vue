<template>
    <div class="wrapper">
        <swiper :options="swiperOption">
            <swiper-slide v-for="item of swiperList" :key="item.id">
                <img class="swiper-image" :src="item.imgUrl"/>
            </swiper-slide>
            <div class="swiper-pagination"  slot="pagination"></div>
        </swiper>
    </div>
</template>

<script>
export default {
  name: 'HomeSwiper',
  data () {
    return {
      swiperOption: {
        pagination: '.swiper-pagination',
        loop: true
      },
      swiperList: [{
        id: '0001',
        imgUrl: 'https://i0.hdslb.com/bfs/archive/197e759e1f07641e19cfeb761ef2014a9c8bb6ed.png@480w_300h.webp'
      },
      {
        id: '0002',
        imgUrl: 'https://i0.hdslb.com/bfs/archive/87dd3e8fd271e7cc4d207ca064ed6f4b5839a137.png@480w_300h.webp'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
    .wrapper >>> .swiper-pagination-bullet-active
        background: #fff !important
    .wrapper
        overflow: hidden
        width: 100%
        height: 0
        padding-bottom: 38%
        background:#fff
    .swiper image
        width:100%
</style>
