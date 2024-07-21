<template>
    <div class="content2">
      <div id="mainBox">
        <div id="box1">
            <div id="post1">
                <div id="pcont">
                    <img :src="p1" class="popic">
                </div>
                <div id="pcont">
                    <p>内容1</p>
                </div>
            </div>
            <div id="post1">
                <div id="pcont">
                <img :src="p2" class="popic">
                </div>
                <div id="pcont">
                    <p>内容2</p>
                </div>
            </div>
            <div id="post1">
                <div id="pcont">
                <img :src="p3" class="popic">
                </div>
                <div id="pcont">
                    <p>内容3</p>
                </div>
            </div>
        </div>
        <div id="box1">
            <div id="post1">
                <div id="pcont">
                    <img :src="p1" class="popic">
                </div>
                <div id="pcont">
                    <p>内容1</p>
                </div>
            </div>
            <div id="post1">
                <div id="pcont">
                <img :src="p2" class="popic">
                </div>
                <div id="pcont">
                    <p>内容2</p>
                </div>
            </div>
            <div id="post1">
                <div id="pcont">
                <img :src="p3" class="popic">
                </div>
                <div id="pcont">
                    <p>内容3</p>
                </div>
            </div>
        </div>
        <div id="box1">
            <div id="post1">
                <div id="pcont">
                    <img :src="p1" class="popic">
                </div>
                <div id="pcont">
                    <p>内容1</p>
                </div>
            </div>
            <div id="post1">
                <div id="pcont">
                <img :src="p2" class="popic">
                </div>
                <div id="pcont">
                    <p>内容2</p>
                </div>
            </div>
            <div id="post1">
                <div id="pcont">
                <img :src="p3" class="popic">
                </div>
                <div id="pcont">
                    <p>内容3</p>
                </div>
            </div>
        </div>
      </div>
    </div>
</template>
<script>
import p1 from '../static/p1.jpg'
import p2 from '../static/p2.jpg'
import p3 from '../static/p3.jpg'
export default{
    data(){
        return{
            p1: p1,
            p2: p2,
            p3: p3,
        }
    }
}
</script>
<style>
.content2{
    grid-column: 1/10;
    grid-row: 3/4;
    background-color: black;
}
#mainBox{
    display: flex;
    flex-direction: column;
    height:1160px;
    margin: 20px;
}
#box1{
    display: flex;
    flex-direction: row;
    height:400px;
}
#post1{
   display: flex;
   flex-direction: column;
   width:400px;
   height:300px;
   margin: 50px;
   gap:50px;
   background-color: rgb(26, 24, 24);
   border-radius: 5px;
}
#pcont{
    display: flex;
    flex-direction: column;
    width:100%;
    height:150px;
}
.popic{
    width:100%;
    height:150px;
}
p{
    color: white;
}
</style>