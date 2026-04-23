<script setup>
  import Home from './components/content/Home.vue';
  import Header from './components/layout/Header.vue';
  
</script>

<template>
    <div class="background-content">
      <Header/>
      <Home/>
    </div>
</template>


<style scoped>
  .background-content{
    background-color: rgb(251, 249, 253);
    height: 100vh;
  }
</style>


