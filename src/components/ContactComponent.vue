<template>
  <div class="row">
    <span class="text-center mt-4">
      Contactanos en nuestras redes sociales
    </span>
  </div>
  <div class="container-fluid container-social ">
    <a class="container-icon shadow-lg" href="https://www.instagram.com/dielecpro/" target="_black">
      <img class="icon" src="../assets/footer/Instagram.svg" alt="instagram">
    </a>
    <a class="container-icon shadow-lg" href="https://api.whatsapp.com/send?phone=50379232974" target="_black">
      <img class="icon" src="../assets/footer/Whatsapp.svg" alt="whatsapp">
    </a>
    <a class="container-icon shadow-lg" href="https://www.facebook.com/dielecpro/" target="_black">
      <img class="icon" src="../assets/footer/Facebook.svg" alt="facebook">
    </a>
    <a class="container-icon shadow-lg" href="https://www.facebook.com/dielecpro/" target="_black">
      <img class="icon" src="../assets/footer/Linkedin.svg" alt="linkedin">
    </a>
  </div>
</template>

<style scoped>
.container-social{
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 15px;
    margin-top: 20px;
    margin-bottom: 20px;
}

.icon{
  width: 60px;
  color: black;
}

.container-icon{
  border-radius: 100%;
  background-color: transparent;
  cursor: pointer;
}
</style>