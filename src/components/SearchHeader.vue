<template>
    <div class="header">
        <div class="header-block block" @click="toPath('/')">Home</div>
        <div class="header-block block" @click="toPath('/search')">Rank Retrival</div>
        <div class="header-block block" @click="toPath('/chatbot')">AI Search</div>
        <!-- <div @click="toPath('/about')">About</div> -->
   </div>
 </template>
 
 <script>
 
 export default {
   name: '',
   components: {
    
   },
   methods:{
    toPath(url){
      this.$router.push({path:url})
    }
   }
 }
 </script>
 
 <style scoped>
    .header{
        width: 100%;
        margin: 0 auto;
        height: 60px;
        display: flex;
        align-items: center;
        justify-content: space-around;
    }
  
    .header-block{
        cursor: pointer;
        flex: 1;
        text-align: center;
        padding: 10px;
        margin: 0 60px;
        border-radius: 5px;
    
    }

    .block{
        background-color: #fff;
        color: #333
    }

    .block:hover{
        background-color: #f0f0f0;
    }
 </style>
 