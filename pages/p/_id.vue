<!--创建路由的方法-->
<template>
    <div>
        <my-header></my-header>
        <div class="note">
            <div class="post">
                 <!--文章正文-->
                <div class="article">
                    <h1 class="title">你若盛开，清风自来</h1>
                    <div class="author">
                        <div class="avatar">
                            <img src="~assets/img/default-avatar.jpg">
                        </div>
                        <div class="info">
                            <nuxt-link class="name" to="name">
                                雪笨笨
                            </nuxt-link>
                            <a href="#" class="btn btn-follow">
                                <i class="fa fa-plus"></i>
                                <span>关注</span>
                            </a>
                            <div class="meta">
                            <span class="publish-time">
                                2018.04.19 14:07
                            </span>
                                <span class="wordage">
                                字数 1199
                            </span>
                                <span class="view-count">
                                阅读 189
                            </span>
                                <span class="comment-count">
                                 评论 10
                            </span>
                                <span class="like-count">
                                 喜欢 559
                            </span>
                            </div>
                        </div>
                    </div>
                    <!--文章正文-->
                    <div class="show-content">
                        <p>在这个吃饭上厕所不带手机感觉缺点啥的时代里，信息的获取简直易如反掌，流量就是王道。信息爆炸的每一天，如何获取有效有价值的知识，作出各种选择，我想，人和人的差距就隐形地体现了出来，不选不知道，一选吓一跳。为什么这么说，以前我拿着手机就是浏览娱乐八卦，或者在某宝上买买买喽，再或者就刷抖音，会让人中毒的短视频，就是在那么一个普通的吃饭时间点，我在翻订阅号文章，看到了长投的推荐文章，正好我最近在阅读理财方面的书籍，也是刚好结束了一期理财培训课，果断点了进去，只用了9.9元，我便开始了一场理财体验之旅。</p><p>我用两天时间读完了小狗钱钱，然后紧接着读了水湄姐姐的作品，获益颇多，我把读后感写下来发给了一位超级友好的学姐，跟她一起探讨了许多问题，包括工作中的压力与职业发展的规划，处在迷茫中的我不断得到学姐的帮助和鼓励，而我自己也通过写成功日记，创立成功相册，一天比一天自信快乐起来。我不知道为什么，但神奇的效果就是这样围绕着我，我每天都过得快乐而充实！</p><p>我知道自己需要一只鹅，哈哈，只有读过小狗钱钱的同学才会懂哦，我就开始从储蓄下手，与此同时，我会关注我们小白训练营的信息更新，从晨读，到打鱼，再到分析和实操，每一步的改变都是自己选择向上的结果，我会为自己打鱼得了负分而暗自伤神，但我会认真思考学姐和班班的讲解去发现问题所在；我会为晨读文章而陷入深思，结合自己的实际情况去努力每天进步一点点;我也会为自己按时完成作业而倍感轻松，但我知道真正的操作在以后的日子里！在成长营里，我看到大家的努力和坚持，看到班班学姐们的耐心和热情，也看到我的不足与缺点，我很庆幸自己能够拥有这样一个圈子，一个让自己变得更加美好的圈子，虽然我身在西北偏远地区，各方面都不够发达，但我从来没有放弃努力，我喜欢阅读，所以会去看订阅号的推荐，故而邂逅了长投学堂，读到了水湄姐姐的书，我渴望像群里的那个人一样拔节生长，因为我想早日实现财务自由，可以自由地选择每一天！</p><p>读过仓央嘉措活佛的一本书，叫做 一切都是最好的安排，我对这句话深信不疑，如果不是最好，那就因为还没有到最后。在最好的安排来临之前，我们能做的就是努力等风来，长投学堂便是来到我身边的清风，让我顺着春天的节奏开始让理财这个生活课题生根发芽，每一天都充满着希望！</p><p>我喜欢小狗钱钱，它陪着吉娅一起成长，收获财富，我的钱钱就是我每一次的努力与改变，从思维模式到行动力，都该有一个新的level了，我相信复利的魔力，更相信不努力的杀伤力！所以，我选择盛开，做优秀的女子，等着清风徐来，只为更加绚烂！感谢小白训练营，感恩所有的老师同学们，也感谢从不安于现状的自己！</p><p>不必焦虑，不必纠结，亦不必心急，做好每一天的自己，对每一个当下负责，牢记，贵有恒，何必三更起五更眠; 最无益，只怕一日曝十日寒。把握好成长的节奏，做自己的主宰，那么，清风自会来！未来，我只会让它更精彩！</p><p>44期9班5组</p><p>519-WANG毕业感言</p>
                    </div>

                </div>
                <!--底部文章分类信息和版权-->
                <div class="show-foot">
                    <nuxt-link to="/note/123" class="notebook">
                        <i class="fa fa-book"></i>日记本
                    </nuxt-link>
                    <div class="copyright">
                        © 著作权归作者所有
                    </div>
                </div>
                <!--文章底部的作者信息-->
                <div class="follow-detail">
                    <div class="info">
                        <div class="avatar">
                            <img src="~assets/img/default-avatar.jpg">
                        </div>
                        <a href="#" class="btn-follow">
                            <i class="fa fa-plus"></i>
                            <span>关注</span>
                        </a>
                        <nuxt-link class="title" to="/u/123">
                            雪笨笨
                        </nuxt-link>
                        <i class="fa fa-venus"></i>
                        <p>写了 1199 字，被 4 人关注，获得了 611 个喜欢</p>
                    </div>
                </div>
                <!--文章底部的喜欢和分享-->
                <div class="meta-bottom">
                    <!--喜欢-->
                    <div class="like" :class="{'islike':islike}" @click="islike=!islike">
                        <div class="like-btn">
                            <a href="javascript:void(0)" class="">喜欢</a>
                        </div>
                        <div class="like-num">
                            <a href="#">50</a>
                        </div>
                    </div>
                    <!--分享-->
                    <div class="share">
                        <a href="#" class="share-btn">
                            <i class="fa fa-weixin weixin"></i>
                        </a>
                        <a href="#" class="share-btn">
                            <i class="fa fa-weibo weibo"></i>
                        </a>
                        <a href="#" class="share-btn">
                            <i class="fa fa-qq qq"></i>
                        </a>
                        <a href="#" class="more-share share-btn">
                            更多分享
                        </a>
                    </div>

                </div>
                <!--留言组件-->
                <my-comment></my-comment>

            </div>


        </div>
    </div>
    </div>
</template>

<script>
    import myComment from '~/components/myComment'
    import myHeader from '~/components/myHeader'
    export default {
        head:{
            title:'简书文章详情页面-创作你的创作',
            meta:[
                {charset:'utf-8'},
                {name:'keyword',content:'文章详情页面'},
                {name:'description',content:'文章页面'}
            ]
        },
        data(){
            return{
                islike:false
            }
        },
        components:{
            myHeader,
            myComment,
        }
    }
</script>

<style scoped>

</style>