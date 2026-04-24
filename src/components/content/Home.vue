<template>
  <div class="container Home-Page  d-flex gap-5 justify-content-between align-items-center">
    <div class="content-left">
        <h6 class="mb-3 border  text-primary h6-spring  rounded-5 py-lg-2 w-50 text-center " style="background-color: gainsboro; ">Spring Collection 2026</h6>
        <h1 class="mb-3 h1-title fw-bolder" style="font-size: 70px;">Discover Your<br> Next Great Read</h1>
        <p class="mb-3 p-des fs-5">Explore thousands of books across all genres. From bestsellers to hidden gems, find your perfect story.</p>
        <div class="d-lg-flex gap-lg-3 d-flex justify-content-lg-start justify-content-center gap-3  mt-lg-5 mt-1">
            <button class="btn rounded-4 btn-primary py-lg-3 px-lg-5 fw-medium">Shop Now</button>
            <button class="btn rounded-4 btn-close-white border fw-medium py-lg-3  px-lg-4">Browse Categories</button>
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
  <hr class="d-lg-block d-none">
<div class="container cate mt-5 mb-5 browse-category">
  <h3 class="fw-bolder">Browse by Category</h3>

  <div class="row g-4 mt-2">

    <div class="col-6 col-md-4 col-lg-2">
      <div class="card text-center h-100">
        <div class="card-header border-0 py-4">
          <i class="bi bg-primary rounded-circle px-3 py-2 text-light fs-3 bi-book"></i>
        </div>
        <div class="card-body">
          <h6>Fiction</h6>
        </div>
      </div>
    </div>

    <div class="col-6 col-md-4 col-lg-2">
      <div class="card text-center h-100">
        <div class="card-header border-0 py-4">
          <i class="bi bg-primary rounded-circle px-3 py-2 text-light fs-3 bi-heart"></i>
        </div>
        <div class="card-body">
          <h6>Romance</h6>
        </div>
      </div>
    </div>

    <div class="col-6 col-md-4 col-lg-2">
      <div class="card text-center h-100">
        <div class="card-header border-0 py-4">
          <i class="bi bg-primary rounded-circle px-3 py-2 text-light fs-3 bi-rocket-takeoff"></i>
        </div>
        <div class="card-body">
          <h6>Sci-Fi</h6>
        </div>
      </div>
    </div>

    <div class="col-6 col-md-4 col-lg-2">
      <div class="card text-center h-100">
        <div class="card-header border-0 py-4">
          <i class="bi bg-primary rounded-circle px-3 py-2 text-light fs-3 bi-patch-question"></i>
        </div>
        <div class="card-body">
          <h6>Self-Help</h6>
        </div>
      </div>
    </div>

    <div class="col-6 col-md-4 col-lg-2">
      <div class="card text-center h-100">
        <div class="card-header border-0 py-4">
          <i class="bi bg-primary rounded-circle px-3 py-2 text-light fs-3 bi-person-arms-up"></i>
        </div>
        <div class="card-body">
          <h6>Mystery</h6>
        </div>
      </div>
    </div>

    <div class="col-6 col-md-4 col-lg-2">
      <div class="card text-center h-100">
        <div class="card-header border-0 py-4">
          <i class="bi bg-primary rounded-circle px-3 py-2 text-light fs-3 bi-cup-hot"></i>
        </div>
        <div class="card-body">
          <h6>Biography</h6>
        </div>
      </div>
    </div>

  </div>
</div>

<div class="container mt-5 featured-books">
  <h3 class="fw-bolder">Featured Books</h3>

  <div class="row g-4 mt-3">

    <!-- Card -->
    <div class="col-12 col-sm-6 col-lg-3">
      <div class="card border-0 shadow rounded-4 h-100">

        <div class="position-relative">
          <img src="https://images.unsplash.com/photo-1589998059171-988d887df646?w=300&h=400&fit=crop"
               class="card-img-top object-fit-cover"
               style="height: 250px;">
          <span class="badge bg-danger position-absolute top-0 start-0 m-3">-20%</span>
        </div>

        <div class="card-body d-flex flex-column">
          <h6 class="fw-bold mb-1">The Art of Computer Programming</h6>
          <p class="text-muted small mb-2">Donald Knuth</p>

          <div class="mb-3 small text-warning">
            ★★★★☆
            <span class="text-muted">(4.8)</span>
          </div>

          <div class="mt-auto d-flex justify-content-between align-items-center">
            <span class="fw-bold text-primary">$89.99</span>
            <button class="btn btn-primary btn-sm rounded-circle"
                    style="width:40px; height:40px;">
              <i class="bi bi-cart"></i>
            </button>
          </div>
        </div>

      </div>
    </div>
    <!-- Card -->
    <div class="col-12 col-sm-6 col-lg-3">
      <div class="card border-0 shadow rounded-4 h-100">

        <div class="position-relative">
          <img src="https://images.unsplash.com/photo-1589998059171-988d887df646?w=300&h=400&fit=crop"
               class="card-img-top object-fit-cover"
               style="height: 250px;">
          <span class="badge bg-danger position-absolute top-0 start-0 m-3">-20%</span>
        </div>

        <div class="card-body d-flex flex-column">
          <h6 class="fw-bold mb-1">The Art of Computer Programming</h6>
          <p class="text-muted small mb-2">Donald Knuth</p>

          <div class="mb-3 small text-warning">
            ★★★★☆
            <span class="text-muted">(4.8)</span>
          </div>

          <div class="mt-auto d-flex justify-content-between align-items-center">
            <span class="fw-bold text-primary">$89.99</span>
            <button class="btn btn-primary btn-sm rounded-circle"
                    style="width:40px; height:40px;">
              <i class="bi bi-cart"></i>
            </button>
          </div>
        </div>

      </div>
    </div>
    <!-- Card -->
    <div class="col-12 col-sm-6 col-lg-3">
      <div class="card border-0 shadow rounded-4 h-100">

        <div class="position-relative">
          <img src="https://images.unsplash.com/photo-1589998059171-988d887df646?w=300&h=400&fit=crop"
               class="card-img-top object-fit-cover"
               style="height: 250px;">
          <span class="badge bg-danger position-absolute top-0 start-0 m-3">-20%</span>
        </div>

        <div class="card-body d-flex flex-column">
          <h6 class="fw-bold mb-1">The Art of Computer Programming</h6>
          <p class="text-muted small mb-2">Donald Knuth</p>

          <div class="mb-3 small text-warning">
            ★★★★☆
            <span class="text-muted">(4.8)</span>
          </div>

          <div class="mt-auto d-flex justify-content-between align-items-center">
            <span class="fw-bold text-primary">$89.99</span>
            <button class="btn btn-primary btn-sm rounded-circle"
                    style="width:40px; height:40px;">
              <i class="bi bi-cart"></i>
            </button>
          </div>
        </div>

      </div>
    </div>
    <!-- Card -->
    <div class="col-12 col-sm-6 col-lg-3">
      <div class="card border-0 shadow rounded-4 h-100">

        <div class="position-relative">
          <img src="https://images.unsplash.com/photo-1589998059171-988d887df646?w=300&h=400&fit=crop"
               class="card-img-top object-fit-cover"
               style="height: 250px;">
          <span class="badge bg-danger position-absolute top-0 start-0 m-3">-20%</span>
        </div>

        <div class="card-body d-flex flex-column">
          <h6 class="fw-bold mb-1">The Art of Computer Programming</h6>
          <p class="text-muted small mb-2">Donald Knuth</p>

          <div class="mb-3 small text-warning">
            ★★★★☆
            <span class="text-muted">(4.8)</span>
          </div>

          <div class="mt-auto d-flex justify-content-between align-items-center">
            <span class="fw-bold text-primary">$89.99</span>
            <button class="btn btn-primary btn-sm rounded-circle"
                    style="width:40px; height:40px;">
              <i class="bi bi-cart"></i>
            </button>
          </div>
        </div>

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

    @media (max-width: 576px){
        .h1-title{
            font-size: 30px !important;
            text-align: center;
        }
        .h6-spring{
            margin: auto;
        }

        .p-des{
            font-size: 10px !important;
            text-align: center;
        }
        .content-left{
            margin-top: -200px !important;
        }
        button{
            font-size: 10px !important;
             border-radius: 10px !important;
        }
        .cate{
          margin-top: -200px !important;
        }
    }

</style>