<script setup>
  import { ref } from 'vue'
  const search = ref('') 
</script>

<template>
  <form role="search">
    <label for="search" class="hidden-visually">Search:</label>
    <input type="text" name="search" id="search" v-model="search">
    <input type="image" class="btnImg" src="https://img.icons8.com/search" alt="Search">
  </form>
</template>

<style>
  .hidden-visually{
    position:absolute;
    overflow: hidden;
    white-space: nowrap;
    margin: 0;
    padding: 0;
    height: 1px;
    width: 1px;
    clip: rect(0 0 0 0);
    clip-path: inset(100%);
  }
</style>


