<template>
    <div class="bg container mb-5 text-center">

        <div class="row">
            <h1>Nuestro Proyectos</h1>
        </div>

        <div class="wrap row d-flex justify-content-center">


            <div class="tile col-12 col-sm-4">
                <img
                    src="https://img.freepik.com/foto-gratis/constructor-electricista-trabajo-examina-conexion-cable-linea-electrica-fuselaje-cuadro-distribucion-industrial-profesional-monos-herramienta-electricista_169016-8635.jpg?w=1060&t=st=1682098560~exp=1682099160~hmac=440d06a81de8440b030966c9ca39baabd51ef0e66591173d7fd73d3fe33fba69"
                />
                <div class="text">
                    <h1>Lorem ipsum.</h1>
                    <h2 class="animate-text">More lorem ipsum bacon ipsum.</h2>
                    <p class="animate-text">
                    Bacon ipsum dolor amet pork belly tri-tip turducken, pancetta bresaola
                    pork chicken meatloaf. Flank sirloin strip steak prosciutto kevin
                    turducken.
                    </p>
                    
                </div>
            </div>

            <div class="tile col-12 col-sm-4">
                <img
                    src="https://images.unsplash.com/photo-1595831708961-1b13c0dd2422?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1201&q=80"
                />
                <div class="text">
                    <h1>Lorem ipsum.</h1>
                    <h2 class="animate-text">More lorem ipsum bacon ipsum.</h2>
                    <p class="animate-text">
                    Bacon ipsum dolor amet pork belly tri-tip turducken, pancetta bresaola
                    pork chicken meatloaf. Flank sirloin strip steak prosciutto kevin
                    turducken.
                    </p>
                    
                </div>
            </div>

            <div class="tile col-12 col-lg-12">
                <img
                    src="https://images.unsplash.com/photo-1513692398020-cbaea622c427?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1170&q=80"
                />
                <div class="text">
                    <h1>Lorem ipsum.</h1>
                    <h2 class="animate-text">More lorem ipsum bacon ipsum.</h2>
                    <p class="animate-text">
                    Bacon ipsum dolor amet pork belly tri-tip turducken, pancetta bresaola
                    pork chicken meatloaf. Flank sirloin strip steak prosciutto kevin
                    turducken.
                    </p>
                    
                </div>
            </div>

        </div>

    </div>
</template>

<script>
</script>

<style scoped>

.wrap {
  margin: 50px auto 0 auto;
  width: 100%;
  display: flex;
  align-items: space-around;
  max-width: 1200px;
}
.tile {
  width: 380px;
  height: 380px;
  margin: 10px;
  background-color: var(--text-primary);
  display: inline-block;
  background-size: cover;
  position: relative;
  cursor: pointer;
  transition: all 0.4s ease-out;
  box-shadow: 0px 35px 77px -17px rgba(0, 0, 0, 0.44);
  overflow: hidden;
  color: var(--color-helper);
}
.tile img {
  height: 100%;
  width: 100%;
  position: absolute;
  top: 0;
  left: 0;
  z-index: 0;
  transition: all 0.4s ease-out;
}
.tile .text {
  /*   z-index:99; */
  position: absolute;
  padding: 30px;
  height: calc(100% - 60px);
}
.tile h1 {
  font-weight: 300;
  margin: 0;
  text-shadow: 2px 2px 10px rgba(0, 0, 0, 0.3);
}
.tile h2 {
  font-weight: 100;
  margin: 20px 0 0 0;
  font-style: italic;
  transform: translateX(200px);
}
.tile p {
  font-weight: 300;
  margin: 20px 0 0 0;
  line-height: 25px;
  /*   opacity:0; */
  transform: translateX(-200px);
  transition-delay: 0.2s;
}
.animate-text {
  opacity: 0;
  transition: all 0.7s ease-in-out;
}
.tile:hover {
  /*   background-color:#99aeff; */
  box-shadow: 0px 35px 60px -17px var(--text-primary);
  transform: scale(1.05);
}
.tile:hover img {
  opacity: 0.5;
}
.tile:hover .animate-text {
  transform: translateX(0);
  opacity: 1;
}
.dots {
  position: absolute;
  bottom: 20px;
  right: 30px;
  margin: 0 auto;
  width: 30px;
  height: 30px;
  color: currentColor;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-around;
}

.dots span {
  width: 5px;
  height: 5px;
  background-color: currentColor;
  border-radius: 50%;
  display: block;
  opacity: 0;
  transition: transform 0.4s ease-out, opacity 0.5s ease;
  transform: translateY(30px);
}

.tile:hover span {
  opacity: 1;
  transform: translateY(0px);
}

.dots span:nth-child(1) {
  transition-delay: 0.05s;
}
.dots span:nth-child(2) {
  transition-delay: 0.1s;
}
.dots span:nth-child(3) {
  transition-delay: 0.15s;
}

</style>