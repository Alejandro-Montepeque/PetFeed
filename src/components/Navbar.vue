<template>
  <nav id="navbar" class="navbar navbar-expand-lg bg-body-tertiary " data-bs-theme="dark">
    <div class="container-fluid">
      <a class="navbar-brand texto-medio" href="#">PetFeed</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavDropdown"
        aria-controls="navbarNavDropdown" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNavDropdown">
        <ul class="navbar-nav">
          <li class="nav-item">
            <a class="nav-link active textos-cortos" aria-current="page" href="#home">Inicio</a>
          </li>
          <li class="nav-item">
            <a class="nav-link textos-cortos" href="#presentation">Producto</a>
          </li>
          <li class="nav-item">
            <a class="nav-link textos-cortos" href="#about_we">Sobre nosotros</a>
          </li>
          <li class="nav-item dropdown">
            <a class="nav-link dropdown-toggle textos-cortos" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
              ¿Quienes somos?
            </a>
            <ul class="dropdown-menu">
              <li><a class="dropdown-item textos-cortos" href="#mision_vision">Mision y Visión</a></li>
              <li><a class="dropdown-item textos-cortos" href="#values">Valores</a></li>
              <li><a class="dropdown-item textos-cortos" href="#objective">Objetivos</a></li>
            </ul>
          </li>
        </ul>
      </div>
      <img src="@/assets/petfeed.jpeg" alt="Logo" width="100" height="">
    </div>
  </nav>
</template>

<script>
import 'bootstrap/dist/css/bootstrap.css';
import 'bootstrap/dist/js/bootstrap.bundle';

export default {
  name: "HeaderNavbar",
};
</script>