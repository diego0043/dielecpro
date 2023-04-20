<template>
  <Carousel class="carousel-margin" :autoplay="4000" :wrap-around="true">
    <Slide v-for="slide in images" :key="slide">
      <div class="carousel__item">
        <img class="img-carousel" :src="slide" alt="" />
      </div>
    </Slide>

    <template #addons> </template>
  </Carousel>
</template>

<script>
  import { defineComponent } from "vue";
  import { Carousel, Pagination, Slide } from "vue3-carousel";

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
          "https://media.gettyimages.com/id/511990814/es/foto/reparaciones-industriales-el%C3%A9ctrica-de.jpg?s=612x612&w=gi&k=20&c=bP5148kxhbCxkfUuYbdIRW3G-lgR6i0EVa6hkit1qMw=",
          "https://media.gettyimages.com/id/1268557129/es/foto/electricistas-cableado-de-una-nueva-construcci%C3%B3n.jpg?s=612x612&w=gi&k=20&c=zWh_AJjlVcI_bH-WQF_Nyw0K_ObF2spoIjMu3hCL5KQ=",
          "https://uploads-ssl.webflow.com/62347826ae55ad163545fc23/631ef9e1d096f19398264c61_types%20of%20electricians.jpg",
        ],
      };
    },
  });
</script>

<style scoped>
  .carousel__item {
    width: 98%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .img-carousel {
    width: 98%;
    height: 100%;
    object-fit: cover;
  }

  .carousel-margin {
    margin-top: 80px;
  }
</style>
