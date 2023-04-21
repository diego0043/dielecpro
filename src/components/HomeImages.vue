<template>
  <Carousel
    class="carousel-margin"
    :autoplay="5000"
    :wrap-around="true"
    :mouse-drag="false"
  >
    <Slide v-for="slide in images" :key="slide">
      <div class="carousel__item">
        <img class="img-carousel" :src="slide" alt="" />
      </div>
    </Slide>
  </Carousel>
</template>

<script>
  import { defineComponent } from "vue";
  import { Carousel, Slide } from "vue3-carousel";

  import "vue3-carousel/dist/carousel.css";

  export default defineComponent({
    name: "Autoplay",
    components: {
      Carousel,
      Slide,
    },

    data() {
      return {
        images: [
          "https://img.freepik.com/foto-gratis/sirva-tecnico-electrico-que-trabaja-centralita-fusibles_169016-24062.jpg?w=2000",
          "https://img.freepik.com/fotos-premium/dos-electricistas-asiaticos-estacion-sistema-electrico-inspeccion-servicio-sitio_10541-5345.jpg?w=2000",
          "https://i0.wp.com/ausinet.com.au/wp-content/uploads/2021/03/Certificate-III-Electrotechnology-Electrician.jpg",
        ],
      };
    },
  });
</script>

<style scoped>
  .carousel__item {
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .img-carousel {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }

  .carousel-margin {
    margin-top: 80px;
  }
</style>
