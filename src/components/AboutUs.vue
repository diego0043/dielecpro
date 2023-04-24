<template>
<div class="container pt-2">
	<div class="row pt-5 pb-4">
		<div class="col-sm-7 col-md-5">
			<img id="uno" src="https://media.istockphoto.com/id/1268557129/es/foto/electricistas-cableado-de-una-nueva-construcci%C3%B3n.jpg?s=612x612&w=0&k=20&c=oSTD7KqJ_rccB7nPvJUQhxkoVpSa4SVJknGwyYrsNDE=" alt="...">
			<img id="dos" src="https://img.freepik.com/fotos-premium/electricistas-trabajan-conectar-cables-electricos-sistema-tablero-distribucion-sistema-electrico-gabinete-control_545582-66.jpg?w=740" alt="">
		</div>
		<div class="col-sm-12 col-md-7">
			<div class="about">
				<h6>Sobre nosotros</h6>
				<h4>Excelentes servicios residenciales y comerciales</h4>
				<p>Todos nuestros servicios están respaldados por nuestra garantía de satisfacción del 100%. Nuestros electricistas pueden instalar cualquier cosa, desde nueva iluminación de seguridad para su exterior hasta un generador para toda la casa que mantendrá sus electrodomésticos funcionando durante un corte de energía. </p>
				<ul>
					<li>
						Disposición eléctrica de servicio completo, diseño 
					</li>
					<li>
						Cableado e instalación/actualizaciones 
					</li>
					<li>
						Soluciones de energía de emergencia (generadores) 
					</li>
					<li>
						Prácticamente cualquier necesidad eléctrica que tenga, ¡solo pregunte! 
					</li>
				</ul>
			</div>
		</div>
	</div>
</div>
<div class="misionvision-uno">
		<div class="row mt-5 pb-5 mb-5">
			<div class="mision1-bg">			
				<div class="mision1">
					<h4 class="mision1-title">MISION</h4>
					<p class="mision1-desciption">Nuestra misión es liderar el mercado ejecutando proyectos de media y baja tensión, así como en el ámbito industrial y comercial a nivel nacional, con soluciones innovadoras y eficientes respaldadas por nuestra experiencia de 10 años. Nos comprometemos con la calidad, cumplimiento de plazos y satisfacción del cliente. Buscamos establecer relaciones duraderas basadas en la confianza, excelencia y ser la opción preferida en el mercado.</p>
				</div>
			</div>
		</div>
		<div class="row mt-5 pb-5 mb-5">
			<div class="vision1-bg">
				<div class="vision1">
					<h4 class="vision1-title">VISION</h4>
					<p class="vision1-desciption">Nuestra misión es liderar el mercado ejecutando proyectos de media y baja tensión, así como en el ámbito industrial y comercial a nivel nacional, con soluciones innovadoras y eficientes respaldadas por nuestra experiencia de 10 años. Nos comprometemos con la calidad, cumplimiento de plazos y satisfacción del cliente. Buscamos establecer relaciones duraderas basadas en la confianza, excelencia y ser la opción preferida en el mercado.</p>
				</div>
			</div>
		</div>
</div>
<div class="mision-dos mt-4">
	<div class="col-sm-10 col-md-6 mb-5 ">
		<div class="mision2" >
			<h4 class="mision2-title">MISION</h4>
			<p class="mision2-desciption">Nuestra misión es liderar el mercado ejecutando proyectos de media y baja tensión, así como en el ámbito industrial y comercial a nivel nacional, con soluciones innovadoras y eficientes respaldadas por nuestra experiencia de 10 años. Nos comprometemos con la calidad, cumplimiento de plazos y satisfacción del cliente. Buscamos establecer relaciones duraderas basadas en la confianza, excelencia y ser la opción preferida en el mercado.</p>
		</div>
	</div>
</div>
<div class="vision-dos mt-4">
	<div class="col-sm-10 col-md-6 mb-5">
		<div class="vision2" >
			<h4 class="vision2-title">VISION</h4>
			<p class="vision2-description">Nuestra visión es ser reconocidos como una empresa innovadora y eficiente, que se destaca por su amplia experiencia en el sector. Buscamos ser la opción preferida de nuestros clientes, ofreciendo soluciones de vanguardia respaldadas por nuestro equipo altamente calificado y actualizados con las últimas tendencias tecnológicas. Aspiramos a mantener relaciones duraderas con nuestros clientes, basadas en la confianza, la calidad, el cumplimiento y la excelencia en cada proyecto que emprendemos.</p>
		</div>
	</div>
</div>
</template>

<script>
</script>

<style>

/* Sobre nosotros*/
#uno{
	width: 130%;

}
#dos{
	width: 75%;
	position: relative;
	z-index: 2;
	bottom: 25%;
	left: -10%;
}
.about{
	height: 90%;
	top: 5%;
	padding: 10%;
	position: relative;
	background: #fff;
	font-family: 'Poppins'pb-2, sans-serif;
}

.about h6{
	color: var(--color-primary);
	font-weight: 700;
}

.about h4{
	color: var(--text-primary);
	font-weight: 900;
}

.about p,ul{
	padding-top: 2%;
	line-height: 30px;
}

.container ul{
	list-style: none;
}

.container li::before{
	content: '⚡';
}

@media (max-width: 900px) {
	#dos{
		bottom: 14%;
	}
}

@media (max-width: 800px) {
	.about{
		top: 5%;
		padding: 7%;
	}
	#dos{
		bottom: 15%;
	}
}

@media (max-width: 700px) {
	#uno{
		width: 90%;
		padding-left: 6%;
	}
	#dos{
		width: 50%;
		left: 0%;
	}
}

/* Mision y Vision*/

.mision1 .mision1-title,.mision2 .mision2-title ,.vision2 .vision2-title {
    font-size: 36px;
    line-height: 46px;
    color: var(--text-primary);
	font-weight: 600;
    font-family: "Poppins", sans-serif;
    position: relative;
    padding: 37px 0 20px 20%;
    margin: 0 0 23px 0;
}

.vision1 .vision1-title{
	font-size: 36px;
    line-height: 46px;
    color: var(--text-primary);
	font-weight: 600;
    font-family: "Poppins", sans-serif;
    position: relative;
    padding: 37px 0 20px 30%;
    margin: 0 0 23px 0;
}

.vision2 .vision2-title,.vision2 .vision2-description{
	text-align: right;
}
.mision1 .mision1-title::before{
    content: '';
    width: 8px;
    height: calc(100% - 8px);
    background-color: var(--color-secondary);
    position: absolute;
    top: 5px;
    left: 0;
}
.vision1 .vision1-title::before{
	content: '';
    width: 8px;
    height: calc(100% - 8px);
    background-color: var(--color-secondary);
    position: absolute;
    top: 5px;
    left: 95%;
}
.mision1,.vision1,.mision2,.vision2{
	padding: 10%;
	position: relative;
	background: #fff;
	font-family: 'Poppins', sans-serif;
}

.mision2 {
	border-radius: 0% 53% 0% 0% / 8% 69% 0% 0%;
}

.vision2 {
	right: -100%;
	border-radius: 69% 0% 0% 8% / 83% 25% 25% 0%;
}

.mision1{
	box-shadow: 5px 5px 15px 1px rgba(0,0,0, 0.5);
}

.vision1{
	box-shadow: -5px 5px 15px 1px rgba(0,0,0, 0.5);
}

.mision1-bg{
	padding: 10%;
	width: 100%;
	top: -10%;
	position: relative;
	background-image: url('https://i.ibb.co/FVtVbkC/d6f811fd0c668b06401e12f22b91eabb-XL1.jpg');	
	background-repeat: no-repeat;
	background-size: cover;
}

.vision1-bg{
	padding: 10%;
	width: 100%;
	top: -10%;
	background-image: url('https://i.ibb.co/FVtVbkC/d6f811fd0c668b06401e12f22b91eabb-XL2.jpg');	
	background-repeat: no-repeat;
	background-size: cover;
}
.mision-dos{
	background-image: url('https://sonarverde.files.wordpress.com/2014/01/banner-electricidad.jpg');	
	background-repeat: no-repeat;
	background-size: cover;
}

.vision-dos{
	background-image: url('https://cdn.euroinnova.edu.es/euroinnova_es/img_destacados/l/Curso-Superior-Intervenciones-Mantenimiento-Instalaciones-Electricas-Edificios.jpg');	
	background-repeat: no-repeat;
	background-size: cover;
}

@media (max-width: 1600px) {
	.misionvision-uno{
		display: none;
	}
	.mision-dos,.vision-dos{
		display: block;
	}
}
@media (max-width: 775px) {

	.misionvision-uno{
		display: contents;
	}
	.mision-dos,.vision-dos{
		display: none;
	}
	.mision1 {
		width: 85%;
		left: 10%;
	}
	.vision1 {
		width: 85%;
		left: 10%;
	}
}
</style>