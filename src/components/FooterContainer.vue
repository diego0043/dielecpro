<template>
  <div class="footer-container container-fluid">
    <div class="row">
      <div class="col-sm-12 col-md-4 col-lg-4 col-xl-4 row-principal">
        <div class="row row-container-footer mb-3">
          <div class="col img-and-title">
            <img class="logo-footer" src="../assets/Vector.svg" alt="" />
            <span class="title-empresa">DIELECPRO</span>
          </div>
        </div>
        <div class="row">
          <div class="col d-flex">
            <span class="text-footer">
              Nuestro personal son expertos en servicios eléctricos, desde
              iluminación y seguridad hasta reparaciones de emergencia. Nos
              mantenemos actualizados con las últimas tendencias y avances en
              tecnología eléctrica para brindar soluciones personalizadas y de
              alta calidad a nuestros clientes.
            </span>
          </div>
        </div>
      </div>
      <div
        class="col-sm-12 col-md-4 col-lg-4 col-xl-4 col-container margin-center"
      >
        <div class="row row-container-footer">
          <div class="col">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="20"
              height="20"
              fill="currentColor"
              class="span-icon"
              viewBox="0 0 16 16"
            >
              <path
                d="M8 16s6-5.686 6-10A6 6 0 0 0 2 6c0 4.314 6 10 6 10zm0-7a3 3 0 1 1 0-6 3 3 0 0 1 0 6z"
              />
            </svg>
            <span class="text-footer-row">23 Av. Sur entre 9na calle oriente</span>
            <br>
            <span class="text-direction"> y calle santa cruz</span>
          </div>
        </div>
        <div class="row row-container-footer">
          <div class="col">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="20"
              height="20"
              fill="currentColor"
              class="span-icon"
              viewBox="0 0 16 16"
            >
              <path
                d="M8 3.5a.5.5 0 0 0-1 0V9a.5.5 0 0 0 .252.434l3.5 2a.5.5 0 0 0 .496-.868L8 8.71V3.5z"
              />
              <path
                d="M8 16A8 8 0 1 0 8 0a8 8 0 0 0 0 16zm7-8A7 7 0 1 1 1 8a7 7 0 0 1 14 0z"
              />
            </svg>
            <span class="text-footer-row"> Lunes - Sabado 8:00 AM - 5:00 PM </span>
          </div>
        </div>
        <div class="row row-container-footer">
          <div class="col">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="20"
              height="20"
              fill="currentColor"
              class="span-icon"
              viewBox="0 0 16 16"
            >
              <path
                fill-rule="evenodd"
                d="M1.885.511a1.745 1.745 0 0 1 2.61.163L6.29 2.98c.329.423.445.974.315 1.494l-.547 2.19a.678.678 0 0 0 .178.643l2.457 2.457a.678.678 0 0 0 .644.178l2.189-.547a1.745 1.745 0 0 1 1.494.315l2.306 1.794c.829.645.905 1.87.163 2.611l-1.034 1.034c-.74.74-1.846 1.065-2.877.702a18.634 18.634 0 0 1-7.01-4.42 18.634 18.634 0 0 1-4.42-7.009c-.362-1.03-.037-2.137.703-2.877L1.885.511z"
              />
            </svg>
            <span class="text-footer-row"> +503 7498 0189 </span>
          </div>
        </div>
        <div class="row">
          <ContactComponent />
        </div>
      </div>
      <div class="col-sm-12 col-md-4 col-lg-4 col-xl-4">
        <div class="col col-container">
          <a href="https://goo.gl/maps/wT275iZwNoXy4X8UA" target="_blank" class="container-img">
            <MapsComponent />
          </a>
        </div>
      </div>
    </div>
    <div class="row row-finaly">
      <div class="col">
        <span class=""
          >© {{ year }} Electrical Services. All Rights Reserved.</span
        >
      </div>
    </div>
  </div>
</template>

<script setup>
  import ContactComponent from "./ContactComponent.vue";
  import MapsComponent from "./MapsComponent.vue";
  const fecha = new Date();
  const year = fecha.getFullYear();
</script>

<style scoped>
  @media screen and (max-width: 768px) {
    .img-and-title {
      margin-left: 15%;
    }

    .text-footer {
      padding: 10px;
      text-align: justify;
    }

    .col-container {
      display: block;
      margin-top: 0px;
    }

    .row-container-footer {
      display: flex;
      margin: 10px;
      width: 100%;
      margin-top: 20px;
    }

    .span-icon {
      margin-left: 10px;
    }

    .text-footer-row{
      margin-left: 15px;
    }

    .row-finaly{
      margin-top: 20px;
    }
  }

  @media screen and (min-width: 768px) {
    .img-and-title {
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: row; /* establecemos la dirección principal en fila */
      margin-top: -20px;
    }

    .text-footer {
      text-align: justify;
    }

    .col-container {
      display: block;
      margin-top: 10px;
    }

    .row-container-footer {
      display: flex;
      margin-top: 100px;
      width: 100%;
      margin-top: 20px;
    }

    .margin-center {
      display: block;
      margin-left: auto;
      margin-top: 3%;
    }

    .span-icon {
      margin-right: 10px;
      margin-left: 35px;
    }

    .row-principal {
      margin-top: 2%;
    }
  }
  .footer-container {
    background-color: #dfdfdf;
    padding: 20px;
    color: black;
  }

  .title-empresa {
    font-size: 20px;
    font-weight: bold;
    margin-left: 6px;
    font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
  }

  .container-img {
    display: block;
    margin-right: auto;
    margin-left: auto;
    width: 300px;
    height: 300px;
    cursor: pointer;
  }

  .row-finaly {
    background-color: #dfdfdf;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: row;
    text-align: center; /* establecemos la dirección principal en fila */
    height: 6vh;
  }

  .logo-footer {
    width: 80px;
    margin-right: 0px;
  }

  .text-direction{
    margin-left: 66px;

  }
</style>
