<template>
    <div>
        <nav class="navbar navbar-fixed-top">
            <div class="width-limit">
                <!--logo-->

                <nuxt-link class="logo" to="/">
                    <img src="~assets/img/nav-logo.png">
                </nuxt-link>
                <!--右上角，写文章-->
                <nuxt-link to="write" class="write-btn">
                    <i class="fa fa-edit">
                        写文章
                    </i>
                </nuxt-link>
                <!--登录用户信息-->
                <div class="user" v-on:mouseenter="enter" @mouseleave="leave">
                    <div class="drop-down">
                        <nuxt-link to="/u/123" class="avatar">
                            <img src="~assets/img/default-avatar.jpg">
                        </nuxt-link>
                    </div>
                    <ul class="drop-menu" v-show="isShow">
                        <li>
                            <nuxt-link to="/user">
                                <i class="fa fa-home"></i>
                                我的主页
                            </nuxt-link>
                        </li>

                        <li>
                            <nuxt-link to="/user/123/like">
                                <i class="fa fa-heart"></i>
                                喜欢的文章
                            </nuxt-link>
                        </li>

                        <li>
                            <nuxt-link to="/bookmarks">
                                <i class="fa fa-bookmark"></i>
                                收藏的文章
                            </nuxt-link>
                        </li>


                        <li>
                            <nuxt-link to="/setting/basic">
                                <i class="fa fa-cog"></i>
                                设置
                            </nuxt-link>
                        </li>

                        <li>
                            <nuxt-link to="/sign-out">
                                <i class="fa fa-sign-out"></i>
                                退出
                            </nuxt-link>
                        </li>

                    </ul>
                </div>
                <!--右上角，登录注册-->
                <!--导航部分-->
                <div class="container">
                    <!--<button class="navbar-toggle">-->
                    <!--<i class="navbar-icon fa fa-bars"></i>-->
                    <!--</button>-->
                    <ul class="nav-list">
                        <!--<li class="navbar-btn" @click="menutextShow">-->
                        <!--<i class="fa fa-bars"></i>-->
                        <!--</li>-->

                        <li>
                            <nuxt-link class="active"
                                       to="/">
                                <i class="fa fa-compass"> </i>
                                <span>发现</span>

                            </nuxt-link>
                        </li>

                        <li>
                            <nuxt-link to="/follow">
                                <i class="fa fa-book"> </i>
                                <span>关注</span>
                            </nuxt-link>
                        </li>

                        <li class="user" @mouseenter="notifyShowenter" @mouseleave="notifyShowleave">
                            <nuxt-link to="/notify">
                                <i class="fa fa-bell-o"> </i>
                                <span>消息</span>
                            </nuxt-link>
                            <!--//消息里面的下拉框-->
                            <ul class="drop-menu" v-show="notifyShow">

                                <li>
                                    <nuxt-link to="/">
                                        <i class="fa fa-comment-o"></i>
                                        评论
                                    </nuxt-link>
                                </li>

                                <li>
                                    <nuxt-link to="/">
                                        <i class="fa fa-envelope-o"></i>
                                        简信
                                    </nuxt-link>
                                </li>

                                <li>
                                    <nuxt-link to="/">
                                        <i class="fa fa-plus-square-o"></i>
                                        关注
                                    </nuxt-link>
                                </li>

                                <li>
                                    <nuxt-link to="/">
                                        <i class="fa fa-heart-o"></i>
                                        喜欢和赞
                                    </nuxt-link>
                                </li>
                            </ul>
                        </li>
                        <li class="search">
                            <form method="post">
                                <input type="text" placeholder="搜索" class="search-input">
                                <a href="#" class="search-btn">
                                    <i class="fa fa-search"></i>
                                </a>
                            </form>
                        </li>

                        <!---->
                        <!---->
                        <!---->
                        <!---->
                        <li class="navbar-btn" @click="navbarBtnShow">
                            <i class="fa fa-bars"></i>
                        </li>
                    </ul>
                    <transition name="fade">
                        <ul class="navbar-content">
                            <li>
                                <nuxt-link to="/" class="active">
                                    发现
                                </nuxt-link>
                            </li>
                            <li>
                                <nuxt-link to="/">
                                    关注
                                </nuxt-link>
                            </li>
                            <li>
                                <nuxt-link to="/">
                                    消息
                                </nuxt-link>
                            </li>
                            <li class="search">
                                <form action="" method="post">
                                    <input type="text" placeholder="搜索" class="search-input">
                                    <a href="#" class="search-btn">
                                        <i class="fa fa-search"></i>
                                    </a>
                                </form>
                            </li>
                        </ul>
                    </transition>
                </div>
            </div>
        </nav>
    </div>
</template>

<script>
    export default {
        name: "myHeader",
        data() {
            return {
                isShow: false,
                notifyShow: false,
                // Show: false,
                count:0
            }


        },
        methods: {
            enter() {
                this.isShow = true;
            },
            leave() {
                this.isShow = false;
            },
            notifyShowenter() {
                this.notifyShow = true;
            },
            notifyShowleave() {
                this.notifyShow = false;
            },
            navbarBtnShow: function () {
                // this.Show = !this.Show;
                this.count++;
                var count=this.count;
                var el=document.querySelector(".navbar-content");
                el.style.transition='0.1s';
                if(count%2==1){
                    el.style.height='224px';
                }else {
                    el.style.height='0'
                }

            }


        }

    }


</script>

<style>
    nav {
        width: 100%;
        height: 56px;
    }

    .navbar {
        margin-bottom: 20px;
        border-bottom: 1px solid #f0f0f0;
        background-color: #fff;
    }

    .navbar:before {
        content: '';
        display: table;
    }

    .navbar-fixed-top {
        position: fixed;
        left: 0;
        top: 0;
        z-index: 9999;
    }

    nav .width-limit {
        min-width: 768px;
        max-width: 1440px;
        /*background-color: red;!*到时候删除*!*/
        margin: 0 auto;
    }

    nav .logo {
        float: left;
        height: 56px;
        display: block;
    }

    nav .logo img {
        max-width: 100%;
        height: 100%;
        display: block;
    }

    nav .write-btn {
        float: right;
        width: 100px;
        height: 40px;
        line-height: 40px;
        margin: 8px 15px 0;
        border-radius: 20px;
        font-size: 15px;
        color: #fff;
        background: #ea6f5a;
        text-align: center;
    }

    nav .write-btn:hover {
        background-color: #ec6149;
        cursor: pointer;
    }

    nav .user {
        position: relative;
        float: right;
    }

    nav .user .avatar {
        position: relative;
        display: block;
        width: 40px;
        height: 40px;
        margin: 8px 28px 8px 20px;
    }

    nav .user:hover {
        background-color: #f5f5f5;
    }

    nav .user .avatar:before {
        content: '';
        position: absolute;
        border-left: 5px solid transparent;
        border-right: 5px solid transparent;
        border-top: 5px solid #999;
        top: 18px;
        right: -14px
    }

    nav .user .avatar img {
        width: 100%;
        height: 100%;
        border-radius: 50%;
        border: 1px solid #eee;
    }

    nav .user .drop-menu {
        position: absolute;
        left: 0;
        box-shadow: 0 0 8px rgba(0, 0, 0, .1);
        min-width: 160px;
        z-index: 999;
        margin: 0;
        padding: 10px 0;
        font-size: 15px;
    }

    nav .user .drop-menu li a {
        padding: 10px 20px;
        line-height: 30px;
        display: block;
    }

    nav .user .drop-menu li a:hover {
        background-color: #f5f5f5;
    }

    nav .user .drop-menu li a i {
        margin-right: 15px;
        color: #ea6f5a;
        width: 20px;
        height: 20px;
        font-size: 20px;
        display: inline-block;
    }

    nav .nav-list {
        float: left;
        margin: 0;
    }

    nav .nav-list:after {
        content: '';
        height: 0;
        display: block;
        visibility: hidden;
        clear: both;
    }

    nav .nav-list > li {
        float: left;
        margin-left: 5px;
    }

    nav .nav-list > li a {
        /*把a设成块级元素*/
        display: block;
        height: 56px;
        line-height: 26px;
        padding: 15px;
    }

    nav .nav-list > li a.active {
        color: #ea6f5a;
        background-color: none !important;
    }

    nav .nav-list > li a:hover {
        background-color: #f5f5f5;
    }

    nav .nav-list > li a i {
        margin-right: 5px;
        font-size: 20px;
    }

    nav .search {
        padding-left: 15px;
        margin-right: 10px;
    }

    nav .search form {
        margin-bottom: 20px;
        position: relative;
        top: 9px;
    }

    nav .search form .search-input {
        width: 240px;
        height: 38px;
        font-size: 14px;
        padding: 0 40px 0 20px;
        border: 1px solid #eee;
        background-color: #eee;
        border-radius: 40px;
        transition: width .5s;
    }

    nav .nav-list .search form .search-input:focus {
        width: 320px;
    }

    nav .nav-list .search form .search-input:focus + .search-btn {
        border-radius: 50%;
        background-color: #969696;
        color: #fff;
    }

    nav .search form .search-btn {
        position: absolute;
        width: 30px;
        height: 30px;
        top: 4px;
        right: 5px;
        color: #969696;
        text-align: center;
        padding: 0;
    }

    nav .nav-list .search form .search-btn:hover {
        background: none;
    }

    nav .nav-list .search form .search-btn i {
        display: block !important;
        font-size: 15px;
        margin: 0;
        text-align: center;
        line-height: 30px;
    }

    /*.navbar-toggle{*/
    /*float: left;*/
    /*padding: 11px 10px;*/
    /*margin-top: 9px;*/
    /*position: relative;*/
    /*margin-right: 15px;*/
    /*margin-bottom: 8px;*/
    /*background-color: transparent;*/
    /*background-image: none;*/
    /*border: 1px solid #ddd;*/
    /*border-radius: 4px;*/
    /*}*/
    /*.navbar-toggle .navbar-icon{*/
    /*width: 22px;*/
    /*}*/

    nav .nav-list .navbar-btn {
        position: absolute;
        top: 10px;
        left: 100px;
        padding: 5px 10px;
        border: 1px solid #ddd;
        border-radius: 5px;
        color: #888888;
        cursor: pointer;
        display: none;
    }

    nav .nav-list .navbar-btn:hover {
        background-color: rgb(247, 247, 247);
    }

    nav .navbar-content {
        height: 0;
        width: 100%;
        display: flex;
        justify-content: center;
        flex-wrap: wrap;
        /*position: fixed;*/
        top: 40px;
        left: 0;
        z-index: 1000;
        background-color: #fff;
    }

    nav .navbar-content li {
        text-align: center;
        width: 100%;
        padding: 15px;
        height: 56px;
        border-bottom: 1px solid #ddd;
    }

    nav .navbar-content li a.active {
        color: #ea6f5a;
    }

    nav .navbar-content .search {
        position: relative;
    }

    nav .navbar-content .search form .search-input {
        width: 100%;
        position: absolute;
        top: -15px;
        left: 0;
    }

    nav .navbar-content .search form .search-btn {
        position: absolute;
        top: -6px;
        right: 5px;
    }

    nav .navbar-content .search form .search-input:focus + .search-btn {
        border-radius: 50%;
        background-color: #969696;
        color: #fff;
    }

    nav .navbar-content .search form .search-btn i {
        /*top: -5px;*/
        display: block !important;
        font-size: 15px;
        margin: 0;
        text-align: center;
        line-height: 20px;
    }


    nav .navbar-content .search form .search-btn {
        position: absolute;
        width: 25px;
        height: 25px;
        top: -8px;
        right: 5px;
        color: #969696;
        text-align: center;
        padding: 0;
    }

    nav .navbar-content li:nth-of-type(2):hover {
        background-color: #f0f0f0;
    }

    nav .navbar-content li:nth-of-type(3):hover {
        background-color: #f0f0f0;
    }
    nav .navbar-content{
        overflow: hidden;
    }

    /*.fade-enter-active, .fade-leave-active {*/
    /*transition: height .1s;*/
    /*}*/
    /*.fade-enter, .fade-leave-to  {*/
    /*height: 0px;*/
    /*}*/
    /*.fade-enter-to,.fade-leave{*/
    /*height: 206px;*/
    /*}*/


    /*媒体查询*/
    @media (max-width: 1440px) {
        nav .nav-list > li a i {
            display: none;
        }

        nav .nav-list .search form .search-input {
            width: 160px;
        }

        nav .nav-list .search form .search-input:focus {
            width: 240px;
        }
    }

    @media (max-width: 1080px) {
        nav .nav-list > li span {
            display: none;
        }

        nav .nav-list > li a i {
            display: block;
        }
    }

    @media (max-width: 768px) {
        nav .nav-list > li:nth-of-type(-n+4) {
            display: none;
        }

        nav .nav-list .navbar-btn {
            display: block;
        }
        nav .navbar-content{
            overflow: hidden;
        }

    }
    @media (min-width: 768px){
        nav .navbar-content{
            display: none;
        }
    }


</style>
