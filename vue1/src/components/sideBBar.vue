<template>
    <div class="sideBBar">
      <div id="sBB1">
        <div id="user-page">
            <div id="ubg">
                <div id="user-avatar">
                    <img :src="userAva" class="ua"> 
                </div>
                <div id="user-name">
                    <p>名字</p>
                </div>
                <div id="user-profile">
                    <p>各种简介</p>
                </div>
            </div>
        </div>
        <div id="recent-comments">
                <div id="r1">
                    <p>近期评论</p>
                </div>
                <div id="r2">
                    <p>评论</p>
                </div>
                <div id="r2">
                    <p>评论</p>
                </div>
                <div id="r2">
                    <p>评论</p>
                </div>
                <div id="r2">
                    <p>评论</p>
                </div>
                <div id="r2">
                    <p>评论</p>
                </div>
        </div>
      </div>
    </div>
</template>
<script>
import userAva from '../static/ua.png'

export default{
    data(){
        return{
            userAva: userAva
        }
    }
}
</script>
<style>
.sideBBar{
    grid-column: 10/13;
    grid-row: 3/4;
    background-color: black;
}
#sBB1{
    display: flex;
    flex-direction: column;
    height:1200px;
    gap:50px;
}
#user-page{
    display: flex;
    flex-direction: column;
    background: linear-gradient(90deg,#FFFFFF 0%,#EE82EE 0%,#00D1FF 100%); 
    height:450px;
    margin: 70px 50px 20px 20px;
}
#recent-comments{
    display: flex;
    flex-direction: column;
    height:450px;
    background-color: rgb(26, 24, 24);
    margin: 0 50px 20px 20px;
}
#ubg{
    display: flex;
    flex-direction: column;
    background-color: rgb(26, 24, 24);
    height: 450px;
    margin: 20px;
}
#user-avatar{
    display: flex;
    height:50px;
    justify-content: center;
    align-items: center;
}
.ua{
    border-radius: 40px;
    width:80px;
    height: 80px;
}
#user-name{
    display: flex;
    height:50px;
    justify-content: center;
    align-items: center;
    margin-top:20px;
}
#user-profile{
    display: flex;
    height:50px;
    justify-content: center;
    align-items: center;
    margin-top:80px;
}
#r1{
    display: flex;
    height:50px;
    justify-content: center;
    align-items: center;
}
#r2{
    display: flex;
    justify-content: center;
    align-items: center;
    height:50px;
    background-color:black;
    margin: 10px;
}
</style>
