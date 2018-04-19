<template>
    <div style="height: 100%">
        <my-header></my-header>
        <p>hello</p>
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
                name:'首页'
            }
        }
    }

</script>

<style scoped>

</style>