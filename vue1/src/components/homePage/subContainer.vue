<template>
  <div class="subContainer">
    <navBar></navBar>
    <content1></content1>
    <content2></content2>
    <sideBBar></sideBBar>
    <content3></content3>
    <footBar></footBar>
  </div>   
</template>
<script>
import navBar from '../navBar.vue'
import content1 from '../content1.vue'
import content2 from '../content2.vue'
import content3 from '../content3.vue'
import sideBBar from '../sideBBar.vue'
import footBar from '../footBar.vue'
export default{
  name: 'subContainer',
  components: {
    navBar,
    content1,
    content2,
    content3,
    sideBBar,
    footBar,
  }
}
</script>
<style>
.subContainer{
    display: grid;
    grid-template-columns: repeat(12,1fr);
    grid-template-rows:100px 600px 1200px 400px 100px;
    width:100vw;
    height:100vh;
}
</style>