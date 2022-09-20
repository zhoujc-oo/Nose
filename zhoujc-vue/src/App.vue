<script>

export default{
  data(){
    return{
      num:0,
      uname:"张三",
      msg:"<h1>标题</h1>"
    };
  },
  methods:{
    changeUname: function (){
      this.uname = "李四"

    },
  },
};
</script>

<template>
 <div>
   <p>{{num}}</p>
   <p>{{uname }}</p>
   <p v-html = "msg"></p>
   <p v-once>{{uname}}</p>
   <button @click = "changeUname">改变名字</button>
 </div>
</template>

<style>


</style>
