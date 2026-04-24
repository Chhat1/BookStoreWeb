<script setup>
  import Home from './components/content/Home.vue';
import Footer from './components/layout/Footer.vue';
  import Header from './components/layout/Header.vue';
  
</script>

<template>
    <div class="background-content">
      <Header/>
      <Home/>
      <Footer/>
    </div>
</template>


<style scoped>
  .background-content{
    background-color: rgb(251, 249, 253);
    height: 150vh;
  }
</style>


