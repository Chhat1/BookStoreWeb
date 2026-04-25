<template>
  <div class="container py-5">

    <!-- HERO -->
    <div class="row align-items-center gy-4">

      <!-- LEFT -->
      <div class="col-12 col-lg-6 text-center text-lg-start">
        <h6 class="mb-3 border text-primary rounded-5 py-2 px-3 d-inline-block"
            style="background-color: gainsboro;">
          Spring Collection 2026
        </h6>

        <h1 class="fw-bolder mb-3 hero-title">
          Discover Your<br class="d-none d-lg-block"> Next Great Read
        </h1>

        <p class="mb-3 text-muted">
          Explore thousands of books across all genres.
        </p>

        

        <div class="d-flex gap-3 mt-4 justify-content-center justify-content-lg-start flex-wrap">
          <button class="btn btn-primary px-4 py-2 rounded-3">
            Shop Now
          </button>
          <button class="btn border px-4 py-2 rounded-3">
            Browse Categories
          </button>
        </div>
      </div>

      <!-- RIGHT -->
      <div class="col-lg-6 d-none d-lg-flex justify-content-center gap-4">
        <div class="card w-50 shadow rounded-4" style="transform: rotate(-8deg);">
          <img class="w-100 rounded-4"
               src="https://images.unsplash.com/photo-1544947950-fa07a98d237f?w=300&h=400&fit=crop">
        </div>

        <div class="card w-50 shadow rounded-4" style="transform: rotate(8deg);">
          <img class="w-100 rounded-4"
               src="https://images.unsplash.com/photo-1543002588-bfa74002ed7e?w=300&h=400&fit=crop">
        </div>
      </div>

    </div>

    <hr class="my-5">

    <!-- BOOKS -->
    <div>
      <h3 class="fw-bolder mb-4 text-center text-lg-start">
        Featured Books
      </h3>

      


        <!-- SEARCH -->
        <div class="d-flex gap-2 mb-5 mt-3 justify-content-center justify-content-lg-start">
          <input v-model="search"
                 @keyup.enter="fetchBooks"
                 type="text"
                 class="form-control shadow-none"
                 placeholder="Search books...">
          <button class="btn btn-primary" @click="fetchBooks">Search</button>
        </div>

        <!-- LOADING -->
      <div v-if="loading" class="text-center">
        <img width="150"
             src="https://img.pikbest.com/png-images/20190918/cartoon-snail-loading-loading-gif-animation_2734139.png!bw700">
      </div>

      <!-- GRID -->
      <div class="row g-4">

        <div v-for="(book, index) in books.slice(0, 8)"
             :key="index"
             class="col-6 col-md-4 col-lg-3">

          <div class="card h-100 border-0 shadow-sm rounded-4">

            <img
              :src="book.cover_i 
                ? `https://covers.openlibrary.org/b/id/${book.cover_i}-M.jpg`
                : 'https://via.placeholder.com/300x400'"
              class="card-img-top"
              style="height: 220px; object-fit: cover;"
            >

            <div class="card-body d-flex flex-column">
              <h6 class="fw-bold mb-1 small">
                {{ book.title }}
              </h6>

              <p class="text-muted small mb-2">
                {{ book.author_name ? book.author_name[0] : 'Unknown' }}
              </p>

              <div class="mt-auto d-flex justify-content-between align-items-center">
                <span class="fw-bold text-primary small">
                  ${{ randomPrice() }}
                </span>

                <button class="btn btn-sm btn-primary rounded-circle"
                        style="width:35px; height:35px;">
                  <i class="bi bi-cart"></i>
                </button>
              </div>
            </div>

          </div>

        </div>

      </div>
    </div>

  </div>
</template>

<script setup>
import { ref, onMounted } from "vue";

const books = ref([]);
const loading = ref(false);
const search = ref("html");

const fetchBooks = async () => {
  loading.value = true;
  try {
    const res = await fetch(`https://openlibrary.org/search.json?q=${search.value}`);
    const data = await res.json();
    books.value = data.docs;
  } catch (err) {
    console.error(err);
  } finally {
    loading.value = false;
  }
};

const randomPrice = () => {
  return (Math.random() * 50 + 10).toFixed(2);
};

onMounted(fetchBooks);
</script>

<style scoped>
.hero-title {
  font-size: 60px;
}

/* MOBILE */
@media (max-width: 576px) {
  .hero-title {
    font-size: 32px;
  }
}
</style>