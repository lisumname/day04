<template>
  <div class="school">
   <h2 @click="showNmae">姓名:{{name}}</h2>
   <h2>性别:{{sex}}</h2>
   <h2>年龄:{{age}}</h2>
  </div>
</template>

<script>
 import {hunhe} from '../mixin.js'
export default {
    name:'MySchool',
    mixins:[hunhe],
    props:['name','age','sex']  //简单接收写法
    // props:{
    //     //指定获取的是什么类型
    //     name:String,
    //     age:Number,
    //     sex:String
    // }

    //接收的同时对数据进行类型限制+默认值的指定+必要性的限制
    // props:{
    //     name:{
    //         type:String,     //name的类型是字符串
    //         required:true  //name是必要的  不会跟default一块使用  这个是必须得传 而defalut是在没传的情况下的默认值
    //     },
    //     age:{
    //         type:Number,
    //         // required:true
    //         default:99   //默认值 就是在没传age属性的时候也会有age属性
    //     },
    //     sex:{
    //         type:String,
    //         required:true
    //     }
    // }
}
</script>

<style>
.school{
    background-image: url('https://gimg2.baidu.com/image_search/src=http%3A%2F%2Fpic1.win4000.com%2Fwallpaper%2F8%2F55402f62682e3.jpg&refer=http%3A%2F%2Fpic1.win4000.com&app=2002&size=f9999,10000&q=a80&n=0&g=0n&fmt=auto?sec=1670086393&t=798c3e9ba1433657df9c4eba57426dec');
   filter: opacity(.6) blur(1px) invert(1) saturate(5) grayscale(1) hue-rotate(90deg) sepia(1) grayscale();
}
</style>
