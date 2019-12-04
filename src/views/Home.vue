<template>
  <div class="home">
    <!-- <img alt="Vue logo" src="../assets/logo.png"> -->
    <input type="text" placeholder="搜索" @input="search" v-model="text">
   <List :dataList="dataList"></List>
 
  </div>
</template>

<script>
// @ is an alias to /src
import List from "../components/List"
export default {
  name: 'home',
  data(){
    return {
      dataList:[
        {
          name:"我的同桌呀",
          msg:"作业写完了？666"
        },
         {
          name:"我的同桌2",
          msg:"hello!在吗"
        },
         {
          name:"我的同桌",
          msg:"作业写完了？666"
        },
         {
          name:"我的同桌2",
          msg:"hello!在吗"
        },
      ],
      text:""
    }
  },
  components: {
    List
  },
  methods:{
    search(){
     this.dataList=this.dataList.filter(item=>{
         return item.name.includes(this.text)
      })
    }
  }
}
</script>
