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
  import img1 from "../assets/home/32970526739.png";
  import img2 from "../assets/home/06v6ZeCY5aW0xl1jQFSwF-transformed-transformed.jpeg";
  import img3 from "../assets/home/OjSLcv7TAFVioIt99RfX5-transformed--HO-iaCY-L-transformed.jpeg";

  export default defineComponent({
    name: "Autoplay",
    components: {
      Carousel,
      Slide,
    },

    data() {
      return {
        images: [img1, img2, img3],
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
