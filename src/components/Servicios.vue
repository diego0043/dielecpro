<template>
<div class="servicios" data-aos="zoom-in-up" data-aos-offset="500" data-aos-duration="1500">
	<div class="item">
		<div class="item-bg">
			<div class="item-bg-img" style="background-image: url(&quot;https://www.virgoingenieros.com/wp-content/uploads/2021/09/LINEAS-AEREAS-DE-BAJA-Y-MEDIA-TENSION-2.jpg&quot;);">
			</div>
			<div class="item-bg-top">
			</div>
		</div>
		<div class="item-contenido">
			<div class="item-titulo">
				<span class="icono">
					<img src="" alt="">
				</span>
				<span class="texto">Instalacion y mantenimiento en lineas en media y baja tensión</span>
			</div>									
		</div>
	</div>

	<div class="item">
		<div class="item-bg">
			<div class="item-bg-img" style="background-image: url(&quot;https://www.josdath.com/wp-content/uploads/2020/07/cropped-instalacion-electrica-vips.jpg&quot;);">
			</div>
			<div class="item-bg-top">
			</div>
		</div>
		<div class="item-contenido">
			<div class="item-titulo">
				<span class="icono">
					<img src="" alt="">
				</span>
				<span class="texto">Instalaciones Industriales, comerciales y residenciales</span>
			</div>
		</div>
	</div>
	
	<div class="item">
		<div class="item-bg">
			<div class="item-bg-img" style="background-image: url(&quot;https://lucera.es/blog/wp-content/uploads/2022/08/mantenimiento-placas-solares.jpg&quot;);">
			</div>
			<div class="item-bg-top">
			</div>
		</div>
		<div class="item-contenido">
			<div class="item-titulo">
				<span class="icono">
					<img src="" alt="">
				</span>
				<span class="texto">Instalacion de generacion fotovoltaica.</span>
			</div>
		</div>
	</div>

	<div class="item">
		<div class="item-bg">
			<div class="item-bg-img" style="background-image: url(&quot;https://func.uncuyo.edu.ar/cache/eficiencia-energetica3_315_600_c.jpg&quot;);">
			</div>
			<div class="item-bg-top">
			</div>
		</div>
		<div class="item-contenido">
			<div class="item-titulo">
				<span class="icono">
					<img rc="" alt="">
				</span>
				<span class="texto">Asesoramiento por consumo de energia electrica</span>
			</div>
		</div>
	</div>
</div>

</template>

<style>
body{
	overflow-x: hidden;
}

.servicios {
    overflow: hidden;
    position: relative;
}

@media (min-width: 1025px) {
    .servicios {
        margin-bottom: -13px;
    }
    .servicios:before,
    .servicios:after {
        content: '';
        display: block;
        position: absolute;
        z-index: 3;
        left: 0;
        width: 100%;
        height: 20px;
        background-color: #ffffff;
        transition: height .13s ease;
    }
    .servicios:before {
        top: 0px;
    }
    .servicios:after {
        bottom: 0px;
    }
    .servicios:hover:before {
        height: 0px;
    }
    .servicios:hover:after {
        height: 1px;
    }
}

@media (max-width: 1024.98px) {
    .servicios {
        margin-left: -15px;
        margin-right: -15px;
    }
    .servicios .item:nth-child(2) {
        margin-left: 0px;
        margin-right: 0px;
    }
	.servicios .item:nth-child(3) {
        margin-left: 0px;
        margin-right: 0px;
    }
}

@media (min-width: 767px) {
    .servicios {
        margin-left: -75px;
        margin-right: -75px;
    }
    .servicios .item:nth-child(2) {
        margin-left: -4px;
        margin-right: -4px;
    }
	.servicios .item:nth-child(3) {
        margin-left: -4px;
        margin-right: -4px;
    }
    .servicios:not(.slick-initialized) {
        display: -webkit-box;
        display: -ms-flexbox;
        display: flex;
        flex-direction: row;
        flex-wrap: nowrap;
        justify-content: flex-start;
        align-content: flex-start;
        align-items: flex-start;
    }
    .servicios .item {
        transition: width 0.13s ease;
        position: relative;
    }
    .servicios .item:not(.active) {
        width: 33.333%;
    }
    .servicios .item:nth-child(4) {
        z-index: 1;
    }
    .servicios .item .item-bg {
        margin-left: -76px;
        width: calc(100% + 76px);
    }
    .servicios .item:nth-child(1) {
        z-index: 3;
    }
    .servicios .item:nth-child(2) {
        z-index: 2;
    }
    .servicios .item:nth-child(3) {
        z-index: 1;
    }
	.servicios .item:nth-child(4) {
        z-index: 0;
    }
    .servicios .item:nth-child(1) {
        padding-left: 70px;
    }
    .servicios .item:nth-child(4) {
        padding-right: 70px;
    }
}

@media (min-width: 769px) and (max-width: 1024px) {
    .servicios {
        margin-left: -52px;
        margin-right: -52px;
    }
}

@media (max-width: 768px) {
    .servicios {
        margin-left: 0;
        margin-right: 0;
    }
}

.item {
    position: relative;
    height: 530px;
}

.item .item-bg {
    position: absolute;
    z-index: 0;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    transform: skew(12deg, 0);
    overflow: hidden;
    background-color: #333333;
}

.item .item-bg:before {
    content: "";
    z-index: 1;
    position: absolute;
    left: -100%;
    top: 0;
    width: 100%;
    height: 100%;
    background: -webkit-gradient(linear, left top, right top, from(rgba(255, 255, 255, 0)), color-stop(50%, rgba(255, 255, 255, 0.25)), to(rgba(255, 255, 255, 0)));
    background: linear-gradient(to right, rgba(255, 255, 255, 0) 0%, rgba(255, 255, 255, 0.25) 50%, rgba(255, 255, 255, 0) 100%);
    transition: 0s ease-in-out;
    pointer-events: none;
    opacity: 0.5;
}

.item .item-bg .item-bg-img {
    position: absolute;
    z-index: 0;
    top: 0;
    left: 0;
    width: 110%;
    height: 100%;
    opacity: 0.6;
    background-size: cover;
    background-position: center top;
    background-repeat: no-repeat;
    transition: opacity 0.2s ease;
    transform: skew(-12deg);
    backface-visibility: hidden;
}

.item .item-bg .item-bg-top {
    position: absolute;
    z-index: 2;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
}

.item .item-bg .item-bg-top:before,
.item .item-bg .item-bg-top:after {
    content: '';
    width: calc(100% + 4px);
    height: 20px;
    background-color: #ffffff;
    display: block;
    position: absolute;
    left: -2px;
    transition: height .13s ease;
}

.item .item-bg .item-bg-top:before {
    top: 0;
}

.item .item-bg .item-bg-top:after {
    bottom: 0;
}

.item .item-contenido {
    position: absolute;
    z-index: 1;
    top: 0;
    left: 5% 0;
    width: 90%;
    height: 100%;
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: center;
    align-content: center;
    align-items: center;
    color: #ffffff;
    text-align: center;
    padding-left: 25px;
    padding-right: 25px;
}

.item .item-titulo {
    font-size: 30px;
    line-height: 1;
    width: 90%;
    font-family: "Poppins", sans-serif;
    font-weight: 600;
    position: relative;
}

.item .item-titulo .icono {
    display: inline-block;
    position: absolute;
    top: -85px;
    left: 50%;
    -webkit-transform: translateX(-50%);
    transform: translateX(-50%);
    z-index: 1;
    opacity: 0.44;
}

.item .item-titulo span {
    position: relative;
    z-index: 2;
}

.item:hover .item-bg {
    overflow: hidden;
}

.item:hover .item-bg:before {
    left: 100%;
    transition: 0.5s ease-in-out;
}

.item:hover .item-bg .item-bg-top:before,
.item:hover .item-bg .item-bg-top:after {
    height: 0;
}

.item.open-info .item-titulo {
    position: static;
}

.item.open-info .item-titulo .icono {
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    margin-top: -25px;
}

@media (max-width: 1229.98px) {
    .item {
        height: 600px;
    }
    .item .item-tit,ulo {
        font-size: 33px;
    }
	.item .item-contenido:nth-child(1){
		padding-left: 0%;
		padding-right: 0%;
	}
}

@media (max-width: 1024px) {
    .item {
        height: 411px;
    }
    .item.slick-slide {
        height: 411px;
    }
    .item .item-titulo {
        font-size: 18px;
    }
    .item .item-titulo .icono {
        top: -53px;
    }
    .item .item-titulo .icono img {
        max-width: 46px;
    }
    .item .item-contenido{
		padding-left: 15px;
		padding-right: 45px;
		
        
    }
    .item .item-bg .item-bg-top:before,
    .item .item-bg .item-bg-top:after {
        display: none;
    }
}

@media (max-width: 768px) {
    .item {
        height: 411px;
    }
    .item.slick-slide {
        height: 411px;
    }
    .item .item-titulo {
        font-size: 20px;
		font-weight: 900;
    }
    .item .item-titulo .icono {
        top: -53px;
    }
    .item .item-titulo .icono img {
        max-width: 46px;
    }
    .item .item-bg {
        -webkit-transform: skew(12deg, 0);
        transform: skew(0deg, 0);
    }
    .item .item-bg .item-bg-img {
        -webkit-transform: skew(0deg);
        transform: skew(0deg);
        width: 100%;
    }
    .item .item-contenido {
        padding-left: 15px;
        padding-right: 15px;
		left: 7%;   
    }
    .item .item-bg {
        -webkit-transform: skew(0deg, 0);
        transform: skew(0deg, 0);
    }
    .item .item-bg .item-bg-top {
        -webkit-transform: skew(0deg, 0);
        transform: skew(0deg, 0);
    }
    .item .item-bg .item-bg-top:before,
    .item .item-bg .item-bg-top:after {
        display: none;
    }
}

@media (max-width: 575px) {
    .item {
        height: 310px !important;
    }
    .item .item-contenido {
		left: 5%;   
    }
}
</style>