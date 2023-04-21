<script setup>
  import { ref } from "vue";
  const refHome = ref(null);
  const refAbout = ref(null);
  const refServices = ref(null);
  const refProjects = ref(null);
  const refContact = ref(null);

  const showRef = (refBtn) => {
    const refBtns = [refHome, refAbout, refServices, refProjects, refContact];
    refBtns.forEach((refBtn) => {
      if (refBtn.value.classList.contains("default-nav-link")) {
        refBtn.value.classList.remove("default-nav-link");
      }
    });
    refBtn.classList.add("default-nav-link");
  };
</script>

<template>
  <nav class="navbar navbar-expand-lg bg-white navbar-large navbar-position">
    <div class="container-fluid">
      <a class="navbar-brand" href="#"
        ><img class="img-brand-movil" src="../assets/Vector.svg" alt="" /><span
          class="title-navbar navbar-brand-movil"
        >
          Dielecpro</span
        ></a
      >
      <button
        class="btn-navbar"
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
              ><img class="img-brand" src="../assets/Vector.svg" alt="" /><span
                class="title-navbar-pc"
                >DIELECPRO</span
              ></a
            >
          </li>
          <li class="nav-item">
            <button
              ref="refHome"
              @click="showRef(refHome)"
              class="default-nav-link nav-link"
              aria-current="page"
              href="#"
            >
              Inicio
            </button>
          </li>
          <li class="nav-item">
            <button
              ref="refAbout"
              @click="showRef(refAbout)"
              class="nav-link"
              href="#"
            >
              Sobre nosotros
            </button>
          </li>
          <li class="nav-item">
            <button
              ref="refServices"
              @click="showRef(refServices)"
              class="nav-link"
              aria-current="page"
              href="#"
            >
              Servicios
            </button>
          </li>
          <li class="nav-item">
            <button
              ref="refProjects"
              @click="showRef(refProjects)"
              class="nav-link"
              aria-current="page"
              href="#"
            >
              Proyectos
            </button>
          </li>
          <li class="nav-item">
            <button
              ref="refContact"
              @click="showRef(refContact)"
              class="nav-link"
              aria-current="page"
              href="#"
            >
              Contacto
            </button>
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

  .navbar-position {
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    z-index: 100;
  }

  @media screen and (max-width: 768px) {
    .title-navbar {
      font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
      font-size: 1.5rem;
      font-weight: bold;
    }
    .navbar-brand-pc {
      display: none;
    }

    .navbar-brand-movil {
      display: block;
      margin-left: 20px;
    }

    .btn-navbar {
      display: block;
      border: none;
      background-color: transparent;
    }

    .navbar-toggler-icon {
      width: 30px;
    }

    .nav-link {
      background-color: transparent;
      border: none;
    }

    .img-brand-pc {
      display: none;
    }

    .img-brand-movil {
      position: absolute;
      margin-left: -5px;
      margin-top: 8px;
      width: 25px;
      height: 25px;
    }
  }

  @media screen and (min-width: 768px) {
    .title-navbar {
      color: var(--color-primary);
      font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
      font-size: 1.5rem;
      font-weight: bold;
    }
    .navbar-brand-pc {
      display: block;
    }

    .navbar-brand-movil {
      display: none;
    }

    .navbar-large {
      height: 100px;
    }

    .btn-navbar {
      display: none;
    }

    .nav-link {
      background-color: transparent;
      border: none;
      position: relative;
      color: #000;
      text-decoration: none;
    }

    .nav-link:hover {
      color: #000;
    }

    .nav-link::before {
      content: "";
      position: absolute;
      display: block;
      width: 100%;
      height: 2px;
      bottom: 0;
      left: 0;
      background-color: #000;
      transform: scaleX(0);
      transition: transform 0.3s ease;
    }

    .nav-link:hover::before {
      transform: scaleX(1);
    }

    .default-nav-link {
      position: relative;
      color: #000;
      text-decoration: none;
    }

    .default-nav-link::before {
      content: "";
      position: absolute;
      display: block;
      width: 100%;
      height: 2px;
      bottom: 0;
      left: 0;
      background-color: var(--color-primary);
      transform: scaleX(1);
    }

    .img-brand-pc {
      position: absolute;
      margin-left: -25px;
      margin-top: 5px;
      width: 30px;
      height: 30px;
    }

    .img-brand-movil {
      display: none;
    }
  }
</style>
