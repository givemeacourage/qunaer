<template>
    <div class="header">
        <div class="header_back"><i class="iconfont iconfanhui"></i></div>
        <div class="haeder_search"><i class="iconfont iconsousuo"></i>  输入城市/景点/游玩主题</div>
        <div class="header_address">北京<i class="iconfont iconjiantouxia"></i></div>
    </div>
</template>

<script>
    export default {
        name: "Header"
    }
</script>

<style scoped lang="less">
// 1rem = 16px
.header{
  width: 100%;
  height:2.6rem;
  background-color: #00bcd4;
  display: flex;
  .header_back{
    width:2.5rem;
    line-height: 2.6rem;
    text-align: center;
    color: #fff;
  }
  .haeder_search{
    flex: 1;
    margin-top: .5rem;
    height: 1.6rem;
    line-height: 1.6rem;
    border: 1px solid #ccc;
    border-radius: 4px;
    color: #f4f4f4;
    padding-left: .5rem;
   
  }
  .header_address{
    width: 4.4rem;
    color: #fff;
    line-height: 2.6rem;
    text-align: center;
  }
}
</style>