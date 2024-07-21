<template>
    <div class="content1">
        <div id="c1">
            <img :src="background" class="bimg"> 
        </div>
    </div> 
</template>
<script>
//content1背景图片
import background from '../static/background.jpg'

export default{
    data(){
        return{
            background: background
        }
    }
}
</script>
<style>
.content1{
  grid-column: 1/13;
  grid-row: 2/3;
  background-color: black;
}
#c1{
    display: flex;
    margin: 0 50px 0 70px;
}
.bimg{
    width:100%;
    height:600px;
}
</style>