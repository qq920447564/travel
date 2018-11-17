<template>
<div>
  <div class="title">热销推荐</div>
  <ul>
    <li class="item border-bottom" v-for="item of recommendList " :key="id">
        <img class="item-img" :src="item.imgUrl"/>
      <div class="item-info">
        <p class="item-title">{{item.desc}}</p>
        <p class="item-desc"> {{item.desc}}</p>
        <button class="item-button">查看详情</button>
      </div>
    </li>
  </ul>
</div>
</template>

<script>
    export default {
        name: "Recommend",
       data(){
          return{
          recommendList:[{
            id:'0001',
            imgUrl:'http://img1.qunarzz.com/sight/p0/1704/c9/c936f3fccfc6d7eda3.img.jpg_200x200_46052773.jpg',
            title:'杜莎夫人蜡像馆',
            desc:'上海有名的杜莎夫人蜡像馆'
          },{
            id:'0002',
            title:'杜莎夫人蜡像馆',
            imgUrl:'http://img1.qunarzz.com/sight/p0/1704/c9/c936f3fccfc6d7eda3.img.jpg_200x200_46052773.jpg',
            desc:'上海有名的杜莎夫人蜡像馆上海有名'
          },{
            id:'0003',
            title:'杜莎夫人蜡像馆',
            imgUrl:'http://img1.qunarzz.com/sight/p0/1704/c9/c936f3fccfc6d7eda3.img.jpg_200x200_46052773.jpg',
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
.item
    overflow: hidden
    display flex
    height 1.9rem
    .item-img
      width:1.7rem
      height:1.7rem
      padding:.1rem
    .item-info
      flex:1
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

      .item-button
        margin-top .16rem
        background: #ff9300
        padding .1rem
        border-radius .06rem
        color #fff
        float left


</style>
