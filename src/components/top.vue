<template>
   <div>
       <div class="indexheader">
           <router-link :to="{path:'/'}">
               <span v-show="ifshow" class="houtui">&lAarr;</span>
           </router-link>
           <slot></slot>
       </div>
   </div>
</template>
<script>
    export default{
        props:['ifshow'],
        data:function () {
            return{}
        }
    }
</script>
<style scoped>
.indexheader{
    position: relative;
    background:#4C566C;
    color: #ffffff;
    height: 50px;
    width:100%;
    font: 20px/50px "微软雅黑";
    text-align: center;
}
    .houtui{
        color: #ffffff;
        position: absolute;
        left: 20px;
        top: 0px;
    }
</style>