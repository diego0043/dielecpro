<script setup>
  import HomeImages from "./components/HomeImages.vue";
  import Navbar from "./components/Navbar.vue";
  import AboutUs from "./components/AboutUs.vue";
  import Services from "./components/Servicios.vue";
  import FooterContainer from "./components/FooterContainer.vue";
  import SocialNetwork from "./components/SocialNetwork.vue";
  import Projects from "./components/Projects.vue";
</script>

<template>
  <Navbar />
  <HomeImages />
  <SocialNetwork />
  <AboutUs/>
  <Services/>
  <Projects />
  <FooterContainer />
</template>

<style scoped></style>
