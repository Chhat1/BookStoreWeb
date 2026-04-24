<template>
  <footer class="bg-dark text-light pt-5 pb-3 mt-5">
    <div class="container">

      <div class="row g-4">

        <!-- Logo + About -->
        <div class="col-12 col-md-6 col-lg-3">
          <h4 class="fw-bold">StoreBook</h4>
          <p class=" text-light">
            Your favorite online bookstore. Find the best books from all categories with amazing prices.
          </p>
        </div>

        
            <!-- Quick Links -->
        <div class="col-6 col-md-3 col-lg-2">
          <h6 class="fw-bold mb-3">Quick Links</h6>
          <ul class="list-unstyled">
            <li><a href="#" class="text-decoration-none text-light">Home</a></li>
            <li><a href="#" class="text-decoration-none text-light">Shop</a></li>
            <li><a href="#" class="text-decoration-none text-light">Categories</a></li>
            <li><a href="#" class="text-decoration-none text-light">Contact</a></li>
          </ul>
        </div>

        <!-- Categories -->
        <div class="col-6 col-md-3 col-lg-2">
          <h6 class="fw-bold mb-3">Categories</h6>
          <ul class="list-unstyled">
            <li><a href="#" class="text-decoration-none text-light">Fiction</a></li>
            <li><a href="#" class="text-decoration-none text-light">Romance</a></li>
            <li><a href="#" class="text-decoration-none text-light">Sci-Fi</a></li>
            <li><a href="#" class="text-decoration-none text-light">Self-Help</a></li>
          </ul>
        </div>
       

        <!-- Contact -->
        <div class="col-12 contact col-md-6 col-lg-3 ">
          <h6 class="fw-bold mb-3 ">Contact</h6>
          <p class="text-light mb-1">📍 Phnom Penh, Cambodia</p>
          <p class="text-light mb-1">📞 +855 12 345 678</p>
          <p class="text-light">✉️ storebook@gmail.com</p>
        </div>

        <!-- Social -->
        <div class="col-12 social col-md-6 col-lg-2">
          <h6 class="fw-bold mb-3">Follow Us</h6>
          <div class="d-lg-flex d-flex justify-content-lg-start justify-content-center gap-3">

            <a href="#" class="text-light fs-5">
              <i class="bi bi-facebook"></i>
            </a>

            <a href="#" class="text-light fs-5">
              <i class="bi bi-instagram"></i>
            </a>

            <a href="#" class="text-light fs-5">
              <i class="bi bi-twitter-x"></i>
            </a>

            <a href="#" class="text-light fs-5">
              <i class="bi bi-youtube"></i>
            </a>

          </div>
        </div>

      </div>

      <hr class="border-secondary mt-4">

      <!-- Bottom -->
      <div class="text-center small text-light">
        © 2026 StoreBook. All rights reserved.
      </div>

    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer"
}
</script>

<style scoped>

a:hover {
  color: #0d6efd !important;
  transition: 0.3s;
}

@media (max-width: 567px){
    .social{
        text-align: center;
    }
    .contact{
        text-align: center;
    }
    
}
</style>