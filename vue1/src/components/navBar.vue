<template>
  <div class="navBar">
    <div id="nav-content">
    <div id="nc-left">
      <div id="lg">
        <router-link to="/home_page/h1">首页</router-link>
      </div>
    </div>
    <div id="nc-right">
      <div class="search_box">
        <input type="text" class="input" placeholder="请输入搜索内容" v-model="searchQuery">
        <input type="button" value="搜索" class="box" @click="search">
      </div>
      <div class="log_reg">
        <button id="lg">
          <router-link to="/entry_page/lg">登录/注册</router-link>
        </button>
      </div>
    </div>
  </div>
  </div>
</template>
<script></script>
<style>
.navBar{
  grid-column: 1/13;
  grid-row: 1/2;
}
#nav-content{
    display:flex;
    height:100%;
    background: linear-gradient(90deg,#FFFFFF 0%,#EE82EE 0%,#00D1FF 100%); 
    align-items: center;
    justify-content: space-between;
}
#nc-left{
    display:flex;
    align-items: center;
    margin: 50px;
}
#nc-right{
    display:flex;
    gap:40px;
    align-items: center;
    margin:50px;
}
.search_box{
    width: 400px;
    height: 40px;
    border:2px solid red;
    margin:auto;
}
.input{
    float:left;
    width:300px;
    height:40px;
    outline: none;
    border:none;
}
.box{
    float:right;
    width:100px;
    height:40px;
    color:white;
    background-color: red;
    border:none;
    outline:none;
}
.box:hover{
    background-color: orangered;
}
#lg{
    display: flex;
    width:100px;
    height:40px;
    background-color: red;
    border: none;
    justify-content: center;
    align-items: center;
}
#lg:hover{
    background-color: orangered;
}
#na{
    color:white;
}
</style>