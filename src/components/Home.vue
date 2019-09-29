<template>
    <div class="home-page">
        <div class="title">hello world</div>
    </div>
</template>
<script>
export default {
    props:{

    },
    components:{

    },
    data(){
        return {
            list:[]//这个数组用来保存列表数据
        }
    },
    computed:{
        total:function()
        {
            return 100*100;
        }
    },
    methods:{

    },
    created(){

    },
    mounted(){
        //今天很郁闷, 写了三行代码,还报错了!!!!!!!
        axios.get("/list").then((res)=>{
            console.log(res.data);
        })
    }
}
</script>
<style scoped lang="">

</style>