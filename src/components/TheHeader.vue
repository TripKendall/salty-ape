<template>
  <header class="main-header">
    <div class="container">
      <nav class="navbar navbar-expand-lg py-0">
        <div class="container-fluid">
          <div class="logo d-flex align-items-center justify-content-between">
            <a class="navbar-brand py-0 me-0" href="#">
              <img src="/images/logo.webp" alt="Salty Ape Vue SPA Template">
            </a>
            <div class="d-block d-lg-none border-0 download-button-wrapper">
              <div class="align-items-center">
                <a class="btn btn-primary get-stared" href="#vue-template">
                  Download
                </a>
              </div>
            </div>
          </div>
          <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav mx-auto mb-2 mb-lg-0">
              <li class="nav-item">
                <a class="nav-link" aria-current="page" href="#">Top</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#leader-board">Leader Board</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#what">What Is This?</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#faq">FAQ</a>
              </li>
            </ul>
            <div class="login d-lg-flex align-items-center">
              <a class="btn btn-primary get-stared" href="#vue-template">Download</a>
            </div>
          </div>
        </div>
      </nav>
    </div>
  </header>
</template>

<style scoped>
.main-header {
  background-color: rgb(255, 255, 255, .75);
  padding: 0 1rem;
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 999;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

.main-header .navbar {
  padding: 0;
}

.main-header .navbar .navbar-brand {
  padding: 0;
}

.main-header .navbar .navbar-brand img {
  width: 100px !important;
}

.main-header .navbar .navbar-toggler {
  border: 0;
  padding: 0;
  width: 30px;
  height: 30px;
  background-color: transparent;
}

.main-header .navbar .navbar-toggler svg {
  width: 100%;
  height: 100%;
}

.main-header .navbar .navbar-collapse {
  padding: 0;
}

.main-header .navbar .navbar-collapse .navbar-nav {
  margin: 0;
}

.main-header .navbar .navbar-collapse .navbar-nav .nav-item {
  margin: 0;
}

.main-header .navbar .navbar-collapse .navbar-nav .nav-item .nav-link {
  padding: 0;
  font-size: 14px;
  font-weight: 500;
  color: #000;
  text-transform: uppercase;
  margin: 0 15px;
}

.main-header .navbar .navbar-collapse .navbar-nav .nav-item .nav-link:hover {
  color: #000;
}

.main-header .navbar .navbar-collapse .navbar-nav .nav-item .nav-link.active {
  color: #000;
}

.main-header .navbar .navbar-collapse .navbar-nav .nav-item .nav-link.active::after {
  content: '';
  position: absolute;
  bottom: -5px;
  left: 0;
  width: 100%;
  height: 2px;
  background-color: #000;
}

.main-header .navbar .navbar-collapse .navbar-nav .nav-item .nav-link.active::before {
  content: '';
  position: absolute;
  bottom: -5px;
  left: 0;
  width: 100%;
}
</style>
