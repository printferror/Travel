<template>
    <div>
        <home-header></home-header>
        <home-swiper></home-swiper>
        <home-icons></home-icons>
        <recommend-icons></recommend-icons>
        <weekend-icons></weekend-icons>
    </div>
</template>

<script>
import HomeHeader from './components/header'
import HomeSwiper from './components/Swiper'
import HomeIcons from './components/icons'
import RecommendIcons from './components/recommend'
import WeekendIcons from './components/weekend'
export default {
  name: 'Home',
  components: {
    HomeHeader,
    HomeSwiper,
    HomeIcons,
    RecommendIcons,
    WeekendIcons
  }
}
</script>

<style>

</style>
