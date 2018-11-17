<template>
  <div>
   <home-header></home-header>
    <home-swiper></home-swiper>
    <home-icons></home-icons>
    <recommend-icons></recommend-icons>
    <home-weekend></home-weekend>
  </div>

</template>

<script>
  import HomeHeader from './components/Header'
  import HomeSwiper from './components/Swiper'
  import HomeIcons from './components/Icons'
  import RecommendIcons from './components/Recommend'
  import HomeWeekend from './components/Weekend'
    export default {
        name: "Home",
      components:{HomeHeader,HomeSwiper,HomeIcons,RecommendIcons,HomeWeekend}
    }
</script>

<style scoped>

</style>
