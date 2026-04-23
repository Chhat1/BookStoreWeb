<template>
  <header>
    <nav class="px-lg-5 px-3 d-flex justify-content-between align-items-center h-100"
    >
      <div class="logo-menu d-flex gap-5 align-items-center">
        <div class="logo"><h4 class="mb-0 text-light">StoreBook</h4></div>

        <ul class="menu nav gap-4 mb-0 d-lg-flex d-none">
          <li>
            <a class="text-decoration-none color-link fs-5" href="">Browse</a>
          </li>
          <li>
            <a class="text-decoration-none color-link fs-5" href=""
              >Bestseller</a
            >
          </li>
          <li>
            <a class="text-decoration-none color-link fs-5" href=""
              >New Arrivale</a
            >
          </li>
          <li>
            <a class="text-decoration-none color-link fs-5" href="">Deals</a>
          </li>
        </ul>
      </div>

      <div class="search-icons d-lg-flex d-none align-items-center gap-5">
        <div class="search">
          <input
            class="form-control shadow-none"
            type="search"
            placeholder="Search books..."
          />
        </div>
        <div class="icons d-flex gap-5">
          <i class="bi fs-3 text-light bi-person"></i>
          <i class="bi fs-3 text-light bi-cart"></i>
        </div>
      </div>


      <!-- Button Search and Menu-Mobile -->
      <div class="d-lg-none d-flex align-content-center align-items-center gap-3">
        <!-- button search -->
          <i class="bi icon-search-mobile bi-search fs-5 text-light fw-bold" data-bs-toggle="offcanvas"
          data-bs-target="#offcanvasTop"
          aria-controls="offcanvasTop"></i>

        <!-- Menu-Mobile -->
        <a
          class="d-lg-none menu-cursor"
          data-bs-toggle="offcanvas"
          data-bs-target="#staticBackdrop"
          aria-controls="staticBackdrop"
        >
          <i class="bi fs-1 text-light bi-list"></i>
        </a>
      </div>

    </nav>


    


      <!-- Offcanvas Menu -->
      <div class="offcanvas offcanvas-start"
        data-bs-backdrop="static"
        tabindex="-1"
        id="staticBackdrop"
        aria-labelledby="staticBackdropLabel"
      >
        <div class="offcanvas-header">
          <h5 class="offcanvas-title" id="staticBackdropLabel">Menu</h5>
          <button
            type="button"
            class="btn-close shadow-none"
            data-bs-dismiss="offcanvas"
            aria-label="Close"
          ></button>
        </div>

        <div class="offcanvas-body">
          <ul class="nav flex-column gap-3">
            <li class="nav-item">
              <a class="nav-link text-dark fs-5 p-0" href="#"
                ><i class="bi bi-house-door me-2"></i> Browse</a
              >
            </li>
            <li class="nav-item">
              <a class="nav-link text-dark fs-5 p-0" href="#"
                ><i class="bi bi-star me-2"></i> Bestseller</a
              >
            </li>
            <li class="nav-item">
              <a class="nav-link text-dark fs-5 p-0" href="#"
                ><i class="bi bi-clock-history me-2"></i> New Arrival</a
              >
            </li>
            <li class="nav-item">
              <a class="nav-link text-dark fs-5 p-0" href="#"
                ><i class="bi bi-tags me-2"></i> Deals</a
              >
            </li>
            <hr />
            <li class="nav-item">
              <a class="nav-link text-dark fs-5 p-0" href="#"
                ><i class="bi bi-person me-2"></i> Account</a
              >
            </li>
            <li class="nav-item">
              <a class="nav-link text-dark fs-5 p-0" href="#"
                ><i class="bi bi-cart me-2"></i> Cart</a
              >
            </li>
          </ul>

          <div class="mt-auto text-center copyright mt-5">
            <hr />
            <p class="text-muted mb-0" style="font-size: 0.85rem">
              &copy; 2026 StoreBook. All rights reserved.
            </p>
            <p class="text-muted" style="font-size: 0.75rem">
              Designed with <i class="bi bi-heart-fill text-danger"></i> by You
            </p>
          </div>
        </div>
      </div>



      <!-- Offcanvas Search Bar -->
      <div
        class="offcanvas offcanvas-top"
        tabindex="-1"
        id="offcanvasTop"
        aria-labelledby="offcanvasTopLabel"
      >
        <div class="offcanvas-header">
          <h5 class="offcanvas-title" id="offcanvasTopLabel">Search</h5>
          <button
            type="button"
            class="btn-close shadow-none"
            data-bs-dismiss="offcanvas"
            aria-label="Close"
          ></button>
        </div>
        <div class="offcanvas-body">
          <!-- Search Input -->
          <div class="input-group">
            <input
              type="search"
              class="form-control shadow-none"
              placeholder="Search products..."
            />
            <button class="btn btn-dark">Search</button>
          </div>
        </div>
      </div>
  </header>
</template>

<script setup>
</script>

<style scoped>
.menu-cursor, .icon-search-mobile, .bi-person, .bi-cart {
  cursor: pointer;
}
* {
  list-style: none;
}

header {
  height: 10vh;
  background: linear-gradient(50deg, #db2777, #dc2626);
}
.color-link {
  color: white;
  transition: all 0.3s ease-in-out;
}
.color-link:hover {
  color: #30091a;
}

@media (max-width: 576px) {
  .offcanvas {
    width: 80% !important;
  }
  .copyright {
    margin-top: 240px !important;
  }
  .offcanvas-top {
    width: 100% !important;
    height: 150px !important;
  }
}

.offcanvas-body .nav-link {
  color: #333;
  transition: all 0.3s ease;
  padding: 12px 15px !important;
  border-radius: 8px;
}

.offcanvas-body .nav-link:hover {
  background-color: #f0f0f0;
  color: #7c3aed;
  padding-left: 20px !important;
}

.offcanvas-body .nav-link i {
  font-size: 1.2rem;
  margin-right: 15px;
  width: 20px;
  text-align: center;
}
</style>