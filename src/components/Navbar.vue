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
          <li class="nav-item navbar-brand-pc ">
            <a class="navbar-brand" href="#"
              ><img class="img-brand-pc" src="../assets/Vector.svg" alt="" /><span
                class="title-navbar-pc"
                >DIELECPRO</span
              ></a
            >
          </li>
          <li class="nav-item ">
            <a
              ref="refHome"
              @click="showRef(refHome)"
              class="default-nav-link nav-link"
              aria-current="page"
              href="#home"
            >
              Inicio
          </a>
          </li>
          <li class="nav-item">
            <a
              ref="refAbout"
              @click="showRef(refAbout)"
              class="nav-link"
              href="#about"
            >
              Sobre nosotros
            </a>
          </li>
          <li class="nav-item">
            <a
              ref="refServices"
              @click="showRef(refServices)"
              class="nav-link"
              aria-current="page"
              href="#services"
            >
              Servicios
            </a>
          </li>
          <li class="nav-item">
            <a
              ref="refProjects"
              @click="showRef(refProjects)"
              class="nav-link"
              aria-current="page"
              href="#projects"
            >
              Proyectos
            </a>
          </li>
          <li class="nav-item">
            <a
              ref="refContact"
              @click="showRef(refContact)"
              class="nav-link"
              aria-current="page"
              href="#contact"
            >
              Contacto
            </a>
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
      margin-top: 7px;
    }
    .navbar-brand-pc {
      display: none;
    }

    .navbar-brand-movil {
      display: flex;
      justify-content: center;
      align-items: center;
      margin-left: 50px;
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
      margin-top: 7px;
      width: 50px;
    }
  }

  @media screen and (min-width: 768px) {
    .title-navbar-pc {
      font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
      font-size: 1.5rem;
      font-weight: bold;
    }
    .navbar-brand-pc {
      display: flex;
      justify-content: center;
      align-items: center;
    }

    .navbar-brand-movil {
      display: none;
    }

    .navbar-large {
      display: flex;
      justify-content: center;
      align-items: flex-start;
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
      margin-left: -90px;
      margin-top: -22px;
      width: 90px;
    }

    .img-brand-movil {
      display: none;
    }
  }
</style>
