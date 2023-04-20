<script setup></script>

<template>
  <nav class="navbar navbar-expand-lg bg-white shadow-sm">
    <div class="container-fluid">
      <a class="navbar-brand" href="#"
        ><span class="title-navbar navbar-brand-movil">Dielecpro</span></a
      >
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarSupportedContent"
        aria-controls="navbarSupportedContent"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div
        class="collapse navbar-collapse container-items"
        id="navbarSupportedContent"
      >
        <ul class="navbar-nav mb-2 mb-lg-0 items-navbar">
          <li class="nav-item navbar-brand-pc">
            <a class="navbar-brand" href="#"
              ><span class="title-navbar">Dielecpro</span></a
            >
          </li>
          <li class="nav-item">
            <a class="nav-link" aria-current="page" href="#">Inicio</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Sobre nosotros</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" aria-current="page" href="#">Servicios</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" aria-current="page" href="#">Galeria</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" aria-current="page" href="#">Contacto</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<style scoped>
  .items-navbar {
    display: flex;
    margin-left: auto;
    margin-right: auto;
  }

  .nav-item {
    margin: 0 15px;
  }

  .title-navbar {
    font-size: 1.5rem;
    font-weight: 700;
  }

  @media screen and (max-width: 768px) {
    .navbar-brand-pc {
      display: none;
    }

    .navbar-brand-movil {
      display: block;
    }
  }

  @media screen and (min-width: 768px) {
    .navbar-brand-pc {
      display: block;
    }

    .navbar-brand-movil {
      display: none;
    }
  }
</style>
