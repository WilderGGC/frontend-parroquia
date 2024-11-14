<template>
  <div>
    <!-- Menu start -->
    <nav class="navbar navbar-expand-lg navbar-dark">
      <!-- Nav container start -->
      <div class="container-fluid">
        <RouterLink class="navbar-brand text-info fw-semibold fs-4" to="/">Parroquia</RouterLink>
        <!-- Nav button -->
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="offcanvas"
          data-bs-target="#menu-lateral"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <!-- Offcanvas main container start -->
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
            <!-- Navbar links -->
            <ul class="navbar-nav d-flex flex-column flex-lg-row align-items-lg-center w-100">
              <li class="nav-item p-3 py-md-1">
                <RouterLink
                  class="nav-link"
                  to="/"
                  exact-active-class="active-link"
                >
                  <i class="bi bi-house"></i> Inicio
                </RouterLink>
              </li>
              <li class="nav-item p-3 py-md-1">
                <RouterLink
                  class="nav-link"
                  to="/about"
                  exact-active-class="active-link"
                >
                  <i class="bi bi-info-circle-fill"></i> Acerca de...
                </RouterLink>
              </li>
              <li class="nav-item p-3 py-md-1 ms-lg-auto">
                <RouterLink
                  class="nav-link"
                  to="/login"
                  exact-active-class="active-link"
                >
                  <i class="bi bi-box-arrow-in-right"></i> Iniciar sesión
                </RouterLink>
              </li>
              <li class="nav-item p-3 py-md-1">
                <RouterLink
                  class="nav-link"
                  to="/register"
                  exact-active-class="active-link"
                >
                  <i class="bi bi-r-square-fill"></i> Registrarse
                </RouterLink>
              </li>
            </ul>
            <!-- Redes sociales -->
            <div class="d-lg-none d-flex justify-content-center align-items-center mt-3">
              <a href="#"> <i class="bi bi-twitter px-2 text-info fs-2"></i> </a>
              <a href="#"><i class="bi bi-facebook px-2 text-info fs-2"></i></a>
              <a href="#"><i class="bi bi-github px-2 text-info fs-2"></i></a>
              <a href="#"><i class="bi bi-whatsapp px-2 text-info fs-2"></i></a>
            </div>
          </div>
        </section>
        <!-- Offcanvas main container end -->
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
.nav-link {
  color: #ffffff;
  text-decoration: none;
  transition: color 0.3s ease, text-decoration 0.3s ease;
}
.nav-link:hover {
  color: white;
  font-size: larger;
}
.active-link {
  color: yellow !important;
  text-decoration: underline;
  text-decoration-color: #0dcaf0;
  text-decoration-thickness: 2px;
}
@media (min-width: 992px) {
  .nav-link.active-link {
    text-decoration: underline;
    text-decoration-color: #0dcaf0;
    text-decoration-thickness: 3px;
  }
}
.offcanvas-body ul.navbar-nav li {
  text-align: left;
}
.offcanvas-body .d-flex a {
  text-decoration: none;
}
@media (max-width: 768px) {
  .navbar-nav > li:hover {
    background-color: #0dcaf0;
  }
}
</style>
