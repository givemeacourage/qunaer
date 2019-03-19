<template>
    <div class="hot-recommend">
        <div class="hot-content"><span class="hot-week">本周热门榜单</span><span class="hot-all">全部榜单<i class="iconfont iconjiantouxia"></i></span></div>
            <div class="hot-wrapper">
                <div  class="hot-img" v-for="(item,index) in imgList" :key="index">
                    <img :src="item.img" alt="">
                    <span class="title">{{item.title}}</span>
                    <span class="price"><strong>{{item.price}}</strong>起</span>
                </div>
            </div>
    </div>
</template>

<script>
export default {
    name: 'recommend',
    data(){
        return {
            imgList:[
                {
                    img:'http://img1.qunarzz.com/sight/p0/201403/11/1f70100804193c28f8b71378c0faa49e.jpg_250x250_719a8492.jpg',
                    title: "户部巷",
                    price: '￥65'
                },
                {
                    img:'http://img1.qunarzz.com/sight/p0/1603/56/56758da4c81e45d990.img.png_250x250_8a58d459.png',
                    title: "武汉东湖风景区",
                    price: '￥30'
                },
                {
                    img:'http://img1.qunarzz.com/sight/p0/201403/11/1f70100804193c28f8b71378c0faa49e.jpg_250x250_719a8492.jpg',
                    title: "黄鹤楼",
                    price: '￥65'
                },
                {
                    img:'http://img1.qunarzz.com/sight/p0/1901/74/74f247ca73aae5f4a3.img.jpg_250x250_4be0a015.jpg',
                    title: "武汉动物园",
                    price: '￥20'
                },
                {
                    img:'http://img1.qunarzz.com/sight/p0/1805/af/af648beb7239c330a3.img.png_250x250_84f636a5.png',
                    title: "武汉花博汇",
                    price: '￥70'
                },
                {
                    img:'http://img1.qunarzz.com/sight/p0/1504/47/4730a0c01664b63d.water.jpg_250x250_5c8de3a0.jpg',
                    title: "武汉海昌极地海洋公园",
                    price: '￥180'
                },
                {
                    img:'http://img1.qunarzz.com/sight/p0/1603/b1/b1da46b5326eb99e90.water.jpg_250x250_fb414d92.jpg',
                    title: "武汉欢乐谷",
                    price: '￥180'
                },
                {
                    img:'http://img1.qunarzz.com/sight/p0/1805/2d/2dbd8192da29dfcda3.img.jpg_250x250_1b1a1721.jpg',
                    title: "木兰天池",
                    price: '￥59'
                }
                
            ]
        }
    }

}
</script>

<style scoped lang="less">
.hot-recommend{
    overflow-x:auto;
    background-color: #fff;
    margin-top: .8rem;
    padding-bottom: .3rem;
    .hot-content{
    height: 2.6rem;
    line-height: 2.6rem;
        .hot-week{
            position: absolute;
            left: .8rem;
        }
        .hot-all{
            position: absolute;
            right: .8rem;
            }
    }
    .hot-wrapper{
        width: 100%;
        white-space: nowrap;
        .hot-img{
            display: inline-block;
            width: 7.4rem;
            margin-left: .8rem;
            margin-right: .8rem;
        img{
            width: 100%;
            height: 100%;
            margin-bottom: .2rem;
        }
        span{
            display: block;
            text-align: center;
        }
        .price{
            margin-top: .2rem;
        }
        .price strong{
            
            color: #ff8300;
        }
    }
    }
}
</style>

