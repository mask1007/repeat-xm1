<template>
    <div style="height: 100%">
        <my-header></my-header>
        <div class="container index">
            <div class="row">
                <!--占16份-->
                <div class="col-xs-16 main">
                    <!--热门专题-->
                    <div class="recommend-collection">
                        <nuxt-link class="collection" to="/collection/123">
                            <img src="~assets/img/c1.jpg">
                            <span name="name">手绘</span>
                        </nuxt-link>

                        <nuxt-link class="collection" to="/collection/123">
                            <img src="~assets/img/c2.jpg">
                            <span name="name">读书</span>
                        </nuxt-link>

                        <nuxt-link class="collection" to="/collection/123">
                            <img src="~assets/img/c3.jpg">
                            <span name="name">社会热点</span>
                        </nuxt-link>

                        <nuxt-link class="collection" to="/collection/123">
                            <img src="~assets/img/c4.jpg">
                            <span name="name">@IT·互联网</span>
                        </nuxt-link>

                        <nuxt-link class="collection" to="/collection/123">
                            <img src="~assets/img/c1.jpg">
                            <span name="name">旅行·在路上</span>
                        </nuxt-link>

                        <nuxt-link class="collection" to="/collection/123">
                            <img src="~assets/img/c2.jpg">
                            <span name="name">历史</span>
                        </nuxt-link>
                        <nuxt-link to="/collection/123" class="more-collection">
                            更多热门专题
                            <i class="fa fa-angle-right"></i>
                        </nuxt-link>
                    </div>
                    <div class="split-line"></div>
                    <!--文章列表-->
                    <div class="list-container">
                        <ul class="note-list">
                            <li class="have-img">
                                <nuxt-link to="/p/123" class="wrap-img">
                                    <img src="~assets/img/note.jpg">
                                </nuxt-link>
                                <div class="content">
                                    <div class="author">
                                        <nuxt-link to="/p/123" class="avatar">
                                            <img src="~assets/img/default-avatar.jpg">
                                        </nuxt-link>
                                        <div class="info">
                                            <nuxt-link to="'/u/123" class="nickname">测试用户</nuxt-link>
                                            <span class="time">04.12 10:18</span>
                                        </div>
                                    </div>
                                    <nuxt-link class="title" to="/p/123">农夫山泉有点甜</nuxt-link>
                                    <div class="abstruct">
                                        忽然觉得最近某个朋友热情起来了。微信里朋友圈开始点赞打招呼了，从不关注我孩子的，居然也问起我的孩子来了。过来喝茶时带着小吃，笑容可掬，春风满面，让人心里暖暖的。就是嘛，我是...
                                    </div>
                                    <div class="meta">
                                        <nuxt-link to="/c/123" class="collection-tag">社会与法</nuxt-link>
                                        <nuxt-link to="/p/123">
                                            <i class="fa fa-eye"></i>
                                            1500
                                        </nuxt-link>
                                        <nuxt-link to="/p/123">
                                            <i class="fa fa-comment"></i>
                                            100
                                        </nuxt-link>
                                        <span>
                                            <i class="fa fa-heart"></i>
                                            20
                                        </span>

                                    </div>
                                </div>

                            </li>
                            <li>

                                <div class="content">
                                    <div class="author">
                                        <nuxt-link to="/p/123" class="avatar">
                                            <img src="~assets/img/default-avatar.jpg">
                                        </nuxt-link>
                                        <div class="info">
                                            <nuxt-link to="'/u/123" class="nickname">测试用户</nuxt-link>
                                            <span class="time">04.12 10:18</span>
                                        </div>
                                    </div>
                                    <nuxt-link class="title" to="/p/123">农夫山泉有点甜</nuxt-link>
                                    <div class="abstruct">
                                        忽然觉得最近某个朋友热情起来了。微信里朋友圈开始点赞打招呼了，从不关注我孩子的，居然也问起我的孩子来了。过来喝茶时带着小吃，笑容可掬，春风满面，让人心里暖暖的。就是嘛，我是...
                                    </div>
                                    <div class="meta">
                                        <nuxt-link to="/c/123" class="collection-tag">社会与法</nuxt-link>
                                        <nuxt-link to="/p/123">
                                            <i class="fa fa-eye"></i>
                                            1500
                                        </nuxt-link>
                                        <nuxt-link to="/p/123">
                                            <i class="fa fa-comment"></i>
                                            100
                                        </nuxt-link>
                                        <span>
                                            <i class="fa fa-heart"></i>
                                            20
                                        </span>

                                    </div>
                                </div>
                            </li>
                            <li class="have-img">
                                <nuxt-link to="/p/123" class="wrap-img">
                                    <img src="~assets/img/note.jpg">
                                </nuxt-link>
                                <div class="content">
                                    <div class="author">
                                        <nuxt-link to="/p/123" class="avatar">
                                            <img src="~assets/img/default-avatar.jpg">
                                        </nuxt-link>
                                        <div class="info">
                                            <nuxt-link to="'/u/123" class="nickname">测试用户</nuxt-link>
                                            <span class="time">04.12 10:18</span>
                                        </div>
                                    </div>
                                    <nuxt-link class="title" to="/p/123">农夫山泉有点甜</nuxt-link>
                                    <div class="abstruct">
                                        忽然觉得最近某个朋友热情起来了。微信里朋友圈开始点赞打招呼了，从不关注我孩子的，居然也问起我的孩子来了。过来喝茶时带着小吃，笑容可掬，春风满面，让人心里暖暖的。就是嘛，我是...
                                    </div>
                                    <div class="meta">
                                        <nuxt-link to="/c/123" class="collection-tag">社会与法</nuxt-link>
                                        <nuxt-link to="/p/123">
                                            <i class="fa fa-eye"></i>
                                            1500
                                        </nuxt-link>
                                        <nuxt-link to="/p/123">
                                            <i class="fa fa-comment"></i>
                                            100
                                        </nuxt-link>
                                        <span>
                                            <i class="fa fa-heart"></i>
                                            20
                                        </span>

                                    </div>
                                </div>

                            </li>
                            <li>
                                <div class="content">
                                    <div class="author">
                                        <nuxt-link to="/p/123" class="avatar">
                                            <img src="~assets/img/default-avatar.jpg">
                                        </nuxt-link>
                                        <div class="info">
                                            <nuxt-link to="'/u/123" class="nickname">测试用户</nuxt-link>
                                            <span class="time">04.12 10:18</span>
                                        </div>
                                    </div>
                                    <nuxt-link class="title" to="/p/123">农夫山泉有点甜</nuxt-link>
                                    <div class="abstruct">
                                        忽然觉得最近某个朋友热情起来了。微信里朋友圈开始点赞打招呼了，从不关注我孩子的，居然也问起我的孩子来了。过来喝茶时带着小吃，笑容可掬，春风满面，让人心里暖暖的。就是嘛，我是...
                                    </div>
                                    <div class="meta">
                                        <nuxt-link to="/p/123">
                                            <i class="fa fa-eye"></i>
                                            1500
                                        </nuxt-link>
                                        <nuxt-link to="/p/123">
                                            <i class="fa fa-comment"></i>
                                            100
                                        </nuxt-link>
                                        <span>
                                            <i class="fa fa-heart"></i>
                                            20
                                        </span>

                                    </div>
                                </div>
                            </li>
                        </ul>

                    </div>
                    <a href="#" class="load-more">阅读更多</a>
            </div>
                <!--占7份，偏移了1份-->
                <div class="col-xs-offset-1 col-xs-7 aside">
                    <div class="row">
                        <!--广告-->
                        <div class="board">
                            <nuxt-link to="/">
                                <img src="~assets/img/ad1.png">
                            </nuxt-link>
                            <nuxt-link to="/">
                                <img src="~assets/img/ad2.png">
                            </nuxt-link>
                            <nuxt-link to="/">
                                <img src="~assets/img/ad3.png">
                            </nuxt-link>
                            <nuxt-link to="/">
                                <img src="~assets/img/ad4.png">
                            </nuxt-link>
                        </div>
                        <!--推荐作者-->
                        <div class="recommended-author">
                            <div class="title">
                                <span>推荐作者</span>
                                <span @click="rotatefa++">
                                     <nuxt-link to="/" class="page-change">
                                    <!--<i :class="[rotate?'fa fa-refresh go':'fa fa-refresh qq']"   ></i>-->
                                         <i class="fa fa-refresh"
                                            :style="{transform:'rotate('+360*rotatefa+'deg)'}"></i>
                                    换一批
                                </nuxt-link>
                                </span>


                            </div>
                            <ul class="recommended-list">
                                <li>
                                    <nuxt-link class="avatar" to="/u/123">
                                        <img src="~assets/img/default-avatar.jpg">
                                    </nuxt-link>
                                    <a href="#" class="follow" @click="followed">
                                        <i class="fa fa-plus"></i>
                                        关注
                                    </a>
                                    <nuxt-link to="/u/123" class="name">
                                        简书用户
                                    </nuxt-link>
                                    <p>写了198.7K字·1.7K喜欢</p>
                                </li>
                                <li>
                                    <nuxt-link class="avatar" to="/u/123">
                                        <img src="~assets/img/default-avatar.jpg">
                                    </nuxt-link>
                                    <a href="#" class="follow"  @click="followed">
                                        <i class="fa fa-plus"></i>
                                        关注
                                    </a>
                                    <nuxt-link to="/u/123" class="name">
                                        简书用户
                                    </nuxt-link>
                                    <p>写了198.7K字·1.7K喜欢</p>
                                </li>
                                <li>
                                    <nuxt-link class="avatar" to="/u/123">
                                        <img src="~assets/img/default-avatar.jpg">
                                    </nuxt-link>
                                    <a href="#" class="follow">
                                        <i class="fa fa-plus"></i>
                                        关注
                                    </a>
                                    <nuxt-link to="/u/123" class="name">
                                        简书用户
                                    </nuxt-link>
                                    <p>写了198.7K字·1.7K喜欢</p>
                                </li>
                                <li>
                                    <nuxt-link class="avatar" to="/u/123">
                                        <img src="~assets/img/default-avatar.jpg">
                                    </nuxt-link>
                                    <a href="#" class="follow">
                                        <i class="fa fa-plus"></i>
                                        关注
                                    </a>
                                    <nuxt-link to="/u/123" class="name">
                                        简书用户
                                    </nuxt-link>
                                    <p>写了198.7K字·1.7K喜欢</p>
                                </li>
                                <li>
                                    <nuxt-link class="avatar" to="/u/123">
                                        <img src="~assets/img/default-avatar.jpg">
                                    </nuxt-link>
                                    <a href="#" class="follow">
                                        <i class="fa fa-plus"></i>
                                        关注
                                    </a>
                                    <nuxt-link to="/u/123" class="name">
                                        简书用户
                                    </nuxt-link>
                                    <p>写了198.7K字·1.7K喜欢</p>
                                </li>
                                <li>
                                    <nuxt-link class="avatar" to="/u/123">
                                        <img src="~assets/img/default-avatar.jpg">
                                    </nuxt-link>
                                    <a href="#" class="follow">
                                        <i class="fa fa-plus"></i>
                                        关注
                                    </a>
                                    <nuxt-link to="/u/123" class="name">
                                        简书用户
                                    </nuxt-link>
                                    <p>写了198.7K字·1.7K喜欢</p>
                                </li>


                            </ul>
                            <nuxt-link to="/" class="find-more">
                                查看更多
                                <i class="fa fa-angle-right"></i>
                            </nuxt-link>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    //导入组件
    import myHeader from '../components/myHeader'
    export default {
        head:{title:'简书-创作你的世界',
            meta:[
                {charset:'utf-8'},
                {name:'keywords',content:'简书首页'},
                {name:'description',content:'简书首页'},
                {name:'author',content:'孔露萍'}
            ]
        },
        //把组件写进来
        components:{
            myHeader
        },
        data(){
            return{
                rotatefa: 0,
            }
        }
    }

</script>

<style scoped>

</style>