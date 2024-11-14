<template>
  <div>
    <!-- menu start -->
    <nav class="navbar navbar-expand-lg navbar-dark">
      <!-- nav container start -->
      <div class="container-fluid">
        <RouterLink class="navbar-brand text-info fw-semibold fs-4" to="/">Parroquia</RouterLink>
        <!-- nav button -->
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="offcanvas"
          data-bs-target="#menu-lateral"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <!-- offcanvas main container start -->
        <section class="offcanvas offcanvas-start" id="menu-lateral" tabindex="-1">
          <div class="offcanvas-header" data-bs-theme="dark">
            <h5 class="offcanvas-title text-info">Parroquia</h5>
            <button
              class="btn-close"
              type="button"
              aria-label="Close"
              data-bs-dismiss="offcanvas"
            ></button>
          </div>
          <div class="offcanvas-body d-flex flex-column justify-content-between px-0">
            <ul class="navbar-nav fs-5 justify-content-evenly">
              <li class="nav-item p-3 py-md-1">
                <RouterLink class="nav-link" to="/"><i class="bi bi-house"></i> Inicio</RouterLink>
              </li>
              <li class="nav-item p-3 py-md-1">
                <RouterLink class="nav-link" to="/about">Acerca de...</RouterLink>
              </li>
            </ul>
            <!-- enalces redes sociales -->
            <div class="d-lg-none align-self-center">
              <a href="#"> <i class="bi bi-twitter px-2 text-info fs-2"></i> </a
              ><a href="#"><i class="bi bi-facebook px-2 text-info fs-2"></i></a
              ><a href="#"><i class="bi bi-github px-2 text-info fs-2"></i></a
              ><a href="#"><i class="bi bi-whatsapp px-2 text-info fs-2"></i></a>
            </div>
          </div>
        </section>
        <!-- offcanvas main container end -->
      </div>
    </nav>
  </div>
</template>
<style scoped>
nav,
.offcanvas {
  background-color: #1e293b;
}
.navbar-toggler {
  border: none;
}
.navbar-toggler:focus {
  outline: none;
  box-shadow: none;
}
@media (max-width: 768px) {
  .navbar-nav > li:hover {
    background-color: #0dcaf0;
  }
}
</style>
