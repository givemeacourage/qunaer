<template>
    <div class="home">
     <v-header></v-header>
     <Swipper></Swipper>
     <Icon></Icon>
     <Recommend></Recommend>
     <Guess></Guess>
    </div>
</template>

<script>
    import Header from '../../components/home/Header'
    import Swipper from '../../components/home/Swipper'
    import Icon from '../../components/home/Icon'
    import Recommend from '../../components/home/Recommend'
    import Guess from '../../components/home/Guess'
    export default {
        name: "Home",
        components:{
            'v-header': Header,
            Swipper,
            Icon,
            Recommend,
            Guess
        }
    }
</script>

<style scoped lang="less">
    .home{
        background-color: #eee
    }
</style>