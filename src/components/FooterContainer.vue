<template>
  <div class="footer-container container-fluid">
    <div class="row">
      <div class="col-sm-12 col-md-4 col-lg-4 col-xl-4 row-principal">
        <div class="row row-container-footer">
          <div class="col">
            <img class="logo-footer" src="../assets/Vector.svg" alt="" />
            <span>DIELECPRO</span>
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
                d="M8 16s6-5.686 6-10A6 6 0 0 0 2 6c0 4.314 6 10 6 10zm0-7a3 3 0 1 1 0-6 3 3 0 0 1 0 6z"
              />
            </svg>
            <span> 8494 Signal Hill Road Manassas, VA, 20110 </span>
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
            <span> Mon-Fri 08:00 AM - 05:00 PM </span>
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
            <span> 1 (800) 765-43-21 </span>
          </div>
        </div>
      </div>
      <div class="col-sm-12 col-md-4 col-lg-4 col-xl-4 col-container">
        <div class="col">
          <span>
            Nuestros electricistas experimentados están altamente capacitados en
            todos los aspectos del servicio eléctrico, desde sistemas de
            iluminación y seguridad para oficinas hasta reparaciones de
            emergencia. Nos aseguramos de mantener a nuestro personal
            actualizado con las últimas tendencias y avances en tecnología
            eléctrica, lo que garantiza que estén preparados para abordar
            cualquier desafío eléctrico con eficiencia y profesionalismo. Puede
            confiar en nosotros para brindarle soluciones personalizadas y de
            alta calidad para sus necesidades eléctricas.
          </span>
        </div>
      </div>
      <div class="col col-container">
        <div class="container-img">
          <MapsComponent />
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
  import MapsComponent from "./MapsComponent.vue";
  const fecha = new Date();
  const year = fecha.getFullYear();
</script>

<style scoped>
  .footer-container {
    background-color: #303442;
    padding: 20px;
    color: white;
  }

  .container-img {
    width: 300px;
    height: 300px;
    margin-top: 5%;
  }

  .col-container {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: row; /* establecemos la dirección principal en fila */
    background-color: #303442;
    margin-top: 0px;
  }

  .row-principal {
    margin-top: 5%;
  }
  .row-container-footer {
    display: flex;
    margin: 10px;
    width: 100%;
    margin-top: 20px;
  }

  .row-finaly {
    background-color: #303442;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: row;
    text-align: center; /* establecemos la dirección principal en fila */
    height: 6vh;
  }

  .logo-footer {
    width: 20px;
    height: 30px;
    margin-right: 10px;
  }

  .span-icon {
    margin-right: 10px;
  }
</style>
