<template>
        <swiper :options="swiperOption" ref="mySwiper" >
            <!-- slides -->
            <swiper-slide class="swiper-slide">
                <div class="icon_wrapper" >
                        <div class="icon-content" v-for="(item, index) in iconlist" :key="index">
                            <img :src="item.imgurl" alt="">
                            <span class="icon-title">{{item.text}}</span>
                        </div>
                </div>
            </swiper-slide>
            <!-- Optional controls -->
            <div class="swiper-pagination"  slot="pagination"></div>
        </swiper>
</template>

<script>
    export default {
        name: "Icon",
        data(){
            return{
                iconlist:[
                    {imgurl:'http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png',text: '景点门票'},
                    {imgurl:'http://img1.qunarzz.com/piao/fusion/1804/5a/13ceb38dcf262f02.png',text:'一日游'},
                    {imgurl:'http://img1.qunarzz.com/piao/fusion/1804/ff/fdf170ee89594b02.png',text:'北京必游'},
                    {imgurl:'http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20191/0334cf5430b9b5505fd79e2b8d7e8670.png',text:'爬长城'},
                    {imgurl:'http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png',text: '景点门票'},
                    {imgurl:'http://img1.qunarzz.com/piao/fusion/1804/5a/13ceb38dcf262f02.png',text:'一日游'},
                    {imgurl:'http://img1.qunarzz.com/piao/fusion/1804/ff/fdf170ee89594b02.png',text:'北京必游'},
                    {imgurl:'http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20191/0334cf5430b9b5505fd79e2b8d7e8670.png',text:'爬长城'},
                    // {imgurl:'http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png',text: '景点门票'},
                   
                ],
                swiperOption: {
                    // some swiper options/callbacks
                    // 所有的参数同 swiper 官方 api 参数
                    // ...
                    pagination: {
                        el:'.swiper-pagination',
                        
                    },
                    // loop: true,
                    // autoplay: true
                }
            }
        }
    }
</script>

<style scoped lang="less">
     .icon_wrapper{
         background-color: #fff;
        height: 10.6rem;
        // overflow: hidden;
        display: flex;
        display: -webkit-flex;
        flex-direction: row;
        flex-wrap: wrap;
        justify-content: space-around;
        .icon-content {
            
            width: 3.6rem;
            margin: .3rem 1rem .1rem  1rem;
            img{
                width: 100%;
            }
            .icon-title{
                display: block;
                font-size: .8rem;
                text-align: center;
            }
        }
        
    }


   
</style>