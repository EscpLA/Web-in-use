<template>
<div id="nav">
    <div class="nav">
        <div class="navLeft">
            <div class="navLeftImg"><a href=""><img src="https://www.adobe.com/content/dam/cc/icons/Adobe_Corporate_Horizontal_Red_HEX.svg" alt=""></a></div>
            <div class="navLeftName"><a href="">Adobe</a></div>
        </div>
        <div class="navMiddle">
            <ul class="navMiddleUl">
                <li id="nav1" v-on:click="ShowMenu"><a>创意和设计<span class="arrow">></span></a></li>
                <li id="nav2"><a href="">营销和商务<span class="arrow">></span></a></li>
                <li id="nav3"><a href="">PDF和电子签名<span class="arrow">></span></a></li>
                <li id="nav4"><a href="">业务解决方案<span class="arrow">></span></a></li>
                <li id="nav5"><a href="">支持<span class="arrow">></span></a></li>
            </ul>
        </div>
        <div class="navRight">
            <div class="navRightImg"><a href=""></a></div>
            <div class="navRightLogIn"><a href>登录</a></div>
        </div>
    </div>
    <ul class="menu" v-show="isShow" >
        <li class="menu1_1" >
            <div class="menuContent">
                <div class="menuContentHead">Creative Cloud 计划</div>
                <ul>
                    <li>
                        <div class="menuContentLiHead">摄影师</div>
                        <div class="menuContentLiText">Lightroom,Photoshop等</div>
                    </li>
                    <li>
                        <div class="menuContentLiHead">中小型企业</div>
                        <div class="menuContentLiText">适用于团队的创意应用程序和服务</div>
                    </li>
                    <li>
                        <div class="menuContentLiHead">企业</div>
                        <div class="menuContentLiText">适用于大型组织的解决方案</div>
                    </li>
                </ul>
                <button class="menuBtn">查看所有的计划和定价</button>
            </div>
        </li>
        <li class="menu1_2">
            <div class="menuContent">
                <div class="menuContentHead">特色产品</div>
                <ul>
                    <li>
                        <div class="menuContentLiHead">Photoshop</div>
                        <div class="menuContentLiText">图像编辑和设计</div>
                    </li>
                    <li>
                        <div class="menuContentLiHead">Lightroom Classic</div>
                        <div class="menuContentLiText">基于云的照片服务</div>
                    </li>
                    <li>
                        <div class="menuContentLiHead">Illustrator</div>
                        <div class="menuContentLiText">矢量图形和插图</div>
                    </li>
                    <li>
                        <div class="menuContentLiHead">Premiere Pro</div>
                        <div class="menuContentLiText">视频编辑和制作</div>
                    </li>
                    <li>
                        <div class="menuContentLiHead">XD</div>
                        <div class="menuContentLiText">用户体验设计和原型创建</div>
                    </li>
                    <li>
                        <div class="menuContentLiText">查看所有产品</div>
                    </li>
                </ul>
                <button></button>
            </div>
        </li>
        <li class="menu1_3">
            <div class="menuContentHead">探索</div>
                <ul>
                    <li>
                        <div class="menuContentLiText">照片</div>
                    </li>
                    <li>
                        <div class="menuContentLiText">图像设计</div>
                    </li>
                    <li>
                        <div class="menuContentLiText">视频</div>
                    </li>
                    <li>
                        <div class="menuContentLiText">UI和UX</div>
                    </li>
                    <li>
                        <div class="menuContentLiText">3D</div>
                    </li>
                    <li>
                        <div class="menuContentLiHead">Adobe Max</div>
                        <div class="menuContentLiText">点播观看</div>
                    </li>
                  
                </ul>
        </li>
    </ul>
</div>
</template>

<script>
import Vue from 'vue'
export default {
    name :'nav',
}
var isShow;    // eslint-disable-line no-unused-vars

var nav = new Vue({    // eslint-disable-line no-unused-vars
    el:'#nav',
    data:{
      isShow: false
    },
    methods:{
        Showmenu : function(){
            this.isShow=!isShow;
        }
    }
})

</script>
