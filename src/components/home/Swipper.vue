<template>
    <div class="swiper_wrapper">
        <swiper :options="swiperOption" ref="mySwiper" >
            <!-- slides -->
            <swiper-slide>
                <img src="http://img1.qunarzz.com/piao/fusion/1811/31/da037478f37cf202.jpg_750x200_fe28d396.jpg" alt="">
            </swiper-slide>
            <swiper-slide>
                <img src="http://img1.qunarzz.com/piao/fusion/1812/d1/cd4f32e924a5a302.jpg_750x200_3d492837.jpg" alt="">
            </swiper-slide>
            <swiper-slide>
                <img src="http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20193/278a88f18f1523eec8c52f650522be68.jpg_750x200_bc365244.jpg" alt="">
            </swiper-slide>

            <!-- Optional controls -->
            <div class="swiper-pagination"  slot="pagination"></div>

        </swiper>
    </div>
</template>

<script>
    export default {
        name: "Swipper",
        data() {
            return {
                swiperOption: {
                    // some swiper options/callbacks
                    // 所有的参数同 swiper 官方 api 参数
                    // ...
                    pagination: {
                        el:'.swiper-pagination',
                    },
                    loop: true,
                    autoplay: true
                }
            }
        }

    }
</script>

<style scoped lang="less" >

 .swiper_wrapper {
    overflow: hidden;
    height: 0;
    padding-bottom: 8rem;
    background-color:#fff;
    img{
       height: 8rem;
    }
 }
 

</style>