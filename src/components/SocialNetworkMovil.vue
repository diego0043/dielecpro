<template>
  <link
    href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css"
    rel="stylesheet"
  />
  <div class="floating-container" @mouseleave="hideMenu">
    <div
      class="floating-button"
      @click="toggleMenu"
      @keydown.enter.space="toggleMenu"
      :tabindex="isMenuVisible ? '0' : ''"
      :aria-expanded="isMenuVisible"
    >
      <i class="fa fa-globe"></i>
    </div>
    <div
      class="element-container"
      v-show="isMenuVisible"
      @keydown.escape="hideMenu"
      :aria-hidden="!isMenuVisible"
    >
      <a
        href="https://www.instagram.com/dielecpro/"
        class="instagram"
        target="_blank"
        @keydown.enter="hideMenu"
      >
        <span class="float-element tooltip-left">
          <i class="icon fa fa-instagram"></i>
        </span>
      </a>

      <a
        href="https://api.whatsapp.com/send?phone=50379232974"
        target="_blank"
        @keydown.enter="hideMenu"
      >
        <span class="float-element tooltip-left">
          <i class="icon fa fa-whatsapp"></i>
        </span>
      </a>
    </div>
  </div>
</template>

<script>
import { defineComponent, ref } from "vue";
export default defineComponent({
  name: "FloatingMenu",
  setup() {
    const isMenuVisible = ref(false);
    const buttonRef = ref(null);

    function toggleMenu() {
      isMenuVisible.value = !isMenuVisible.value;
      if (isMenuVisible.value) {
        setTimeout(() => {
          buttonRef.value.focus();
        }, 0);
      }
    }

    function hideMenu() {
      if (isMenuVisible.value) {
        isMenuVisible.value = false;
        buttonRef.value.focus();
      }
    }

    return {
      isMenuVisible,
      toggleMenu,
      buttonRef,
      hideMenu,
    };
  },
});
</script>

<style scoped>
@media screen and (max-width: 768px) {

  @-webkit-keyframes come-in {
    0% {
      -webkit-transform: translatey(100px);
      transform: translatey(100px);
      opacity: 0;
    }
    30% {
      -webkit-transform: translateX(-50px) scale(0.4);
      transform: translateX(-50px) scale(0.4);
    }
    70% {
      -webkit-transform: translateX(0px) scale(1.2);
      transform: translateX(0px) scale(1.2);
    }
    100% {
      -webkit-transform: translatey(0px) scale(1);
      transform: translatey(0px) scale(1);
      opacity: 1;
    }
  }
  @keyframes come-in {
    0% {
      -webkit-transform: translatey(100px);
      transform: translatey(100px);
      opacity: 0;
    }
    30% {
      -webkit-transform: translateX(50px) scale(0.4);
      transform: translateX(50px) scale(0.4);
    }
    70% {
      -webkit-transform: translateX(0px) scale(1.2);
      transform: translateX(0px) scale(1.2);
    }
    100% {
      -webkit-transform: translatey(100px) scale(1);
      transform: translatey(100px) scale(1);
      opacity: 1;
    }
  }
  * {
    margin: 0;
    padding: 0;
  }

  .floating-container {
    position: fixed;
    width: 60px;
    height: 100px;
    bottom: 0;
    right: 0;
    margin: 30px 25px;
    z-index: 101;
  }
  .floating-container:hover {
    height: 300px;
  }
  .floating-container:hover .floating-button {
    box-shadow: 0 10px 25px rgba(0, 0, 0, 0.6);
    -webkit-transform: translatey(5px);
    transform: translatey(2px);
    -webkit-transition: all 0.3s;
    transition: all 0.3s;
  }
  .floating-container:hover .element-container .float-element:nth-child(1) {
    -webkit-animation: come-in 0.4s forwards 0.2s;
    animation: come-in 0.4s forwards 0.2s;
  }
  .floating-container:hover .element-container .float-element:nth-child(2) {
    -webkit-animation: come-in 0.4s forwards 0.4s;
    animation: come-in 0.4s forwards 0.4s;
  }
  .floating-container .floating-button {
    /**Boton principal */
    position: absolute;
    width: 65px;
    height: 65px;
    background: var(--text-primary);
    bottom: 0;
    border-radius: 50%;
    left: 0;
    right: 0;
    margin: auto;
    color: var(--color-helper);
    line-height: 65px;
    text-align: center;
    font-size: 30px;
    z-index: 100;
    box-shadow: 0 10px 25px -5px rgba(60, 60, 59, 0.41);
    cursor: pointer;
    -webkit-transition: all 0.3s;
    transition: all 0.3s;
  }
  .floating-container .float-element {
    position: relative;
    display: block;
    border-radius: 50%;
    width: 50px;
    height: 50px;
    margin: 10px auto;
    color: white;
    font-weight: 500;
    text-align: center;
    line-height: 50px;
    z-index: 0;
    opacity: 0;
    -webkit-transform: translateY(100px);
    transform: translateY(100px);
  }
  .floating-container .float-element .icon {
    vertical-align: middle;
    font-size: 25px;
  }
  .floating-container .float-element:nth-child(1) {
    background: var(--text-primary);
    box-shadow: 0 20px 20px -10px var(--text-primary);
  }
}
@media screen and (min-width: 768px) {
    .floating-container {
      display: none;
    }
  }
</style>