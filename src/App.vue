<script setup>
  import HomeImages from "./components/HomeImages.vue";
  import Navbar from "./components/Navbar.vue";
  import AboutUs from "./components/AboutUs.vue";
  import Services from "./components/Servicios.vue";
  import FooterContainer from "./components/FooterContainer.vue";
  import SocialNetwork from "./components/SocialNetwork.vue";
  import SocialNetworkMovil from "./components/SocialNetworkMovil.vue";
  import Projects from "./components/Projects.vue";
</script>

<template>
  <Navbar />
  <HomeImages id="home" />
  <SocialNetworkMovil />
  <SocialNetwork />
  <AboutUs />
  <Services />
  <Projects />
  <FooterContainer id="contact" />
</template>

<style scoped></style>
