<template>
  <div class="wrap">
  <swiper :options="swiperOption" ref="mySwiper"  >
    <!-- slides -->
    <swiper-slide v-for="item of swiperList" :key="item.id">
      <img class="swiper-img" :src="item.imgUrl" />
    </swiper-slide>
    <div class="swiper-pagination"  slot="pagination"></div>
    <!--<div class="swiper-button-prev" slot="button-prev"></div>-->
    <!--<div class="swiper-button-next" slot="button-next"></div>-->
    <!--<div class="swiper-scrollbar"   slot="scrollbar"></div>-->
  </swiper>
  </div>
</template>

<script>
    export default {
        name: "HomeSwiper",
      data(){
          return{
            swiperOption:{
              pagination:'.swiper-pagination',
              loop:'true'
            },
            swiperList:[{
              id:'001',
              imgUrl:'http://img1.qunarzz.com/piao/fusion/1710/15/898d6d74e9b06202.jpg_750x200_89b4509e.jpg'
            },{
              id:'002',
              imgUrl:'http://img1.qunarzz.com/piao/fusion/1809/2d/0d7dc3400a50b502.jpg_750x200_4ca95dd4.jpg'
            }]
          }
      }
    }
</script>

<style lang="stylus" scoped>
  .wrapper >>> .swiper-pagination-bullet-active
     background: #fff
  .wrapper
    overflow :hidden
    width: 100%
    height:0
    padding-bottom: 31.25%
    background :#eaeaea
   .swiper-img
    width:100%
</style>
