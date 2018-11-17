<template>
<div>
  <div class="title">周末去哪儿</div>
  <ul>
    <li class="item border-bottom" v-for="item of recommendList " :key="item.id">
       <div class="item-img-wrapper">
        <img class="item-img" :src="item.imgUrl"/>
       </div>
      <div class="item-info">
        <p class="item-title">{{item.desc}}</p>
        <p class="item-desc"> {{item.desc}}</p>
      </div>
    </li>
  </ul>
</div>
</template>

<script>
    export default {
        name: "Weekend",
       data(){
          return{
          recommendList:[{
            id:'0001',
            imgUrl:'http://img1.qunarzz.com/sight/source/1511/ea/7f43191b747bb9.jpg_r_640x214_f58e829d.jpg',
            title:'杜莎夫人蜡像馆',
            desc:'上海有名的杜莎夫人蜡像馆'
          },{
            id:'0002',
            title:'杜莎夫人蜡像馆',
            imgUrl:'http://img1.qunarzz.com/sight/source/1511/ea/7f43191b747bb9.jpg_r_640x214_f58e829d.jpg',
            desc:'上海有名的杜莎夫人蜡像馆上海有名'
          },{
            id:'0003',
            title:'杜莎夫人蜡像馆',
            imgUrl:'http://img1.qunarzz.com/sight/source/1511/ea/7f43191b747bb9.jpg_r_640x214_f58e829d.jpg',
            desc:'上海有名的杜莎夫人蜡像馆'
          }]

      }
       }
    }
</script>

<style lang="stylus" scoped>
  @import '~@/assets/styles/mixins.styl'
.title
    line-height .8rem
    background #eee
    text-indent .2rem
 .item-img-wrapper
   overflow:hidden
   height 0
   padding-bottom 33.9%
  .item-img
    width:100%
  .item-info
    padding .1rem
    min-width :0
    .item-title
      line-height .54rem
      font-size .32rem
      ellipse()
    .item-desc
      line-height .4rem
      color:#ccc
      ellipse()

</style>
