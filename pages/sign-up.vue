<template>
    <div class="sign">
        <!--logo-->
        <div class="logo">
            <nuxt-link to="/">
                <img src="~assets/img/logo.png">
            </nuxt-link>
        </div>
        <!--主体部分-->
        <div class="main">
            <!--title-->
            <div class="title">
                <h4>
                    <nuxt-link  to="/sign-in">
                        登录
                    </nuxt-link>
                    <b>·</b>
                    <nuxt-link class="active" to="/sign-up">
                        注册
                    </nuxt-link>
                </h4>
            </div>
            <!--form表单-->
            <div class="js-form">
                <form method="post">
                    <div class="input-prepend">
                        <input type="text" placeholder="你的昵称">
                        <i class="fa fa-user"></i>
                    </div>
                    <div class="input-prepend">
                        <input type="text" placeholder="手机号">
                        <i class="fa fa-phone"></i>
                    </div>
                    <div class="input-prepend ssm">
                        <input type="text" placeholder="手机验证码">
                        <i class="fa fa-shield"></i>
                        <a href="#" class="send-ssm">发送验证码</a>
                    </div>
                    <div class="input-prepend">
                        <input type="text" placeholder="密码">
                        <i class="fa fa-lock"></i>
                    </div>

                    <button class="sign-up-btn">注册</button>
                    <p class="sign-up-msg">
                        点击 “注册” 即表示您同意并愿意遵守简书
                        <a href="#">用户协议</a> 和 <a href="#">隐私政策</a> 。
                    </p>
                </form>
            </div>
            <!--第三方的登录-->
            <div class="more-sign">
                <p class="">社交账号直接注册</p>
                <ul class="">
                    <li>
                        <nuxt-link to="/">
                            <i class="weixin fa fa-weixin"></i>
                        </nuxt-link>
                    </li>

                    <li>
                        <nuxt-link to="/">
                            <i class="qq fa fa-qq"></i>
                        </nuxt-link>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
       //修改当前页面的默认模板为sign.vue
        //如果不选，默认就是default.vue
        layout:'sign',
        //设置页面的标题以及描述、关键字等元信息
        head:{
            title:'注册-简书',
            meta:[
                {charset:'utf-8'},
                {name:'keywords',content:'注册页面'},
                {name:'description',content:'注册简书'},
                {name:'author',content:'孔露萍'}
            ]
        },
        data(){
            return{}
        }
    }
</script>

<style>

</style>