<template>
  <div class="container Home-Page mt-5 d-flex gap-5 justify-content-between align-items-center">
    <div class="content-left">
        <h6 class="mb-3 border  text-primary    rounded-5 py-lg-2 w-50 text-center " style="background-color: gainsboro; ">Spring Collection 2026</h6>
        <h1 class="mb-3 fw-bolder" style="font-size: 70px;">Discover Your<br> Next Great Read</h1>
        <p class="mb-3 fs-5">Explore thousands of books across all genres. From bestsellers to hidden gems, find your perfect story.</p>
        <div class="d-flex gap-3 mt-5">
            <button class="btn rounded-4 btn-primary py-3 px-5 fw-medium">Shop Now</button>
            <button class="btn rounded-4 btn-close-white border fw-medium py-3 px-4">Browse Categories</button>
        </div>
    </div>
    <div class="content-right d-lg-flex d-none  align-items-center gap-5">
        <div class="card rounded-4 w-50" style="transform: rotate(-10deg);">
            <div class="card-header p-4">
                <img class="rounded-4" width="100%" src="https://images.unsplash.com/photo-1544947950-fa07a98d237f?w=300&h=400&fit=crop" alt="">
            </div>
            <div class="card-body">
                <h5>The Midnight Library</h5>
                <p>Matt Haig</p>
            </div>
        </div>
        <div class="card rounded-4 w-50" style="transform: rotate(10deg);">
            <div class="card-header p-4">
                <img class="rounded-4" width="100%" src="https://images.unsplash.com/photo-1543002588-bfa74002ed7e?w=300&h=400&fit=crop" alt="">
            </div>
            <div class="card-body">
                <h5>Project Hail Mary</h5>
                <p>Andy Weir</p>
            </div>
        </div>
    </div>
  </div>
</template>

<script setup>

</script>

<style scoped>
    *{
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }

    .Home-Page{
        height: 60vh !important;
    }

</style>