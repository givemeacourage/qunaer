<template >
    <div class="guess">
        <div class="guess-title">猜你喜欢</div>
        <div class="guess-wrapper" v-for="(item,index) in guessList" :key="index">
            <img :src="item.url" alt="">
            <div class="guess-content">
                <span class="title">{{item.title}}</span>
                <span>{{item.comment}}</span>
                <span class="price-content"><strong class="price">￥<strong class="large">{{item.price}}</strong></strong>起</span>
                <span class="address">{{item.address}}</span>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name: 'guess',
    data(){
        return {
            guessList:[
                {
                    url:"http://img1.qunarzz.com/sight/p0/1603/56/56758da4c81e45d990.img.png_200x200_bbb543fa.png",
                    title: '武汉东湖风景区',
                    comment: '1180条评论',
                    price: '30',
                    address: '武昌区'
                },
                 {
                    url:"http://img1.qunarzz.com/sight/p0/1501/10/1012e4a2c398409c.water.jpg_200x200_366b12f8.jpg",
                    title: '云雾山',
                    comment: '1307条评论',
                    price: '55',
                    address: '黄陂区'
                },
                 {
                    url:"http://img1.qunarzz.com/sight/p0/1504/89/892ea25a5d7d77cd.water.jpg_200x200_1760e424.jpg",
                    title: '胜天农庄',
                    comment: '444条评论',
                    price: '195',
                    address: '黄陂区'
                },
                 {
                    url:"http://img1.qunarzz.com/sight/p0/1805/af/af648beb7239c330a3.img.png_200x200_05da91a0.png",
                    title: '武汉花博汇',
                    comment: '1104条评论',
                    price: '70',
                    address: '汉阳区'
                }
            ]
        }
    }
}
</script>

<style scoped lang="less">
    .guess{
        background-color: #fff;
        padding:0 .8rem;
        .guess-title{
            height: 3rem;
            line-height: 3rem;
        }
        .guess-wrapper{
            margin-bottom: .8rem;
            display: flex;
            img{
                width: 7.4rem;
                 height: 7.4rem;
                 margin-right: .8rem;
            }
            .guess-content{
                position:relative;
                flex: 1;
                span{
                    display: block;
                    margin-bottom: .8rem;
                }
                .title{
                    margin-top: .8rem;
                }
                .price-content .price{
                    color: #ff8300;   
                    .large{
                        font-size: 1.2rem;
                    }
                }
                .address{
                    position: absolute;
                    right:.8rem;
                    bottom: 1.2rem;
                }
            }
        }
        
    }
</style>

