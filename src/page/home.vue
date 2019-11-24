<template>
    <div class="home-page">
        <v-header></v-header>
        <ul class="nav">
            <li v-for="item in arrList" :key="item"><img :src="item.imgUrl"><span>{{item.name}}</span></li>
        </ul>
    </div>
</template>
<script>
import Header from '@/components/header'
import WebImg from '@/assets/web.png'
import WebService from '@/assets/webservice.png'
import MoveImg from '@/assets/move.png'
import DataImg from '@/assets/data.png'
import DownloadImg from '@/assets/download.png'
export default {
    data(){
        return{
            arrList:[]
        }
    },
    mounted(){
        this.arrList = [{
            imgUrl:WebImg,
            name:'前端开发'
        },{
            imgUrl:WebService,
            name:'后端开发'
        },{
            imgUrl:MoveImg,
            name:'移动开发'
        },{
            imgUrl:DataImg,
            name:'数据库'
        },{
            imgUrl:DownloadImg,
            name:'云计算'
        }]
    },
    components:{
        'v-header':Header
    }
}
</script>
<style scoped>
    .home-page .nav{
        height: 100px;
        margin-top: 44px;
        background: #F3F5F7;
        overflow-x: scroll;
        white-space: nowrap;
        font-size: 0;
    }
    .nav li{
        width: 88px;
        font-size: 14px;
        color: #2B333B;
        display: inline-block;
        text-align: center;
    } 
    .nav li img{
        display: block;
        width: 32px;
        margin: 20px auto 12px;
    }    
</style>