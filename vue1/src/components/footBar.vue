<template>
    <div class="footBar">
        <div id="f3">
           <p>这是页脚</p>
        </div>
    </div>
</template>
<script></script>
<style>
.footBar{
  grid-column: 1/13;
  grid-row: 5/6;
  background: linear-gradient(90deg,#FFFFFF 0%,#EE82EE 0%,#00D1FF 100%); 
}
#f3{
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100px;
}
</style>