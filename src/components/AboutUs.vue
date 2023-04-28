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

<div class="founder-container contenedor">
	<div class="founder-content">
		<h1>Fundador</h1>
		<div class="carta">
			<img src="https://miro.medium.com/v2/resize:fit:735/1*d_BUs7AyKgRPrICwQGReDA.jpeg" alt="">
			<div class="intro">
				<h3>Papá de Navas</h3>
				<p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Placeat distinctio dolorum animi adipisci magni nisi eveniet numquam iusto quo quod odio consectetur debitis officia ducimus ipsa quas, ipsum nam maxime.</p>
			</div>
		</div>
	</div>
	<!-- <div class="founder-content">
		<h1>Fundador</h1>
		<div class="carta">
			<img src="https://miro.medium.com/v2/resize:fit:735/1*d_BUs7AyKgRPrICwQGReDA.jpeg" alt="">
			<div class="intro">
				<h3>Papá de Navas</h3>
				<p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Placeat distinctio dolorum animi adipisci magni nisi eveniet numquam iusto quo quod odio consectetur debitis officia ducimus ipsa quas, ipsum nam maxime.</p>
			</div>
		</div>
	</div> -->
</div>
</template>

<script>
</script>

<style>

/* Founder styles */

.contenedor {
	margin: 0 70px;
}

.founder-container {
	display: grid;
	grid-template-columns: repeat(2, 1fr);
}

.founder-content h1 {
	text-align: center;
	font-weight: bold;
}

.carta {
	box-shadow: 5px 5px 20px #000;
	overflow: hidden;
	height: 500px;
	margin: 15px;
	position: relative;
}

.carta img {
	width: 100%;
	border-radius: 3px;
	height: 500px;
	object-fit: cover;
}

.carta:hover {
	cursor: pointer;
}

.carta:hover img{
    transform: scale(1.1) rotate(-3deg);
	transition: .5s ease-out;
}

.carta:hover .intro {
	background-color: #000;
	bottom: 0;
}

.carta:hover p {
	visibility: visible;
	opacity: 1;
}

.intro {
	/* height: 200px; */
	width: 100%;
	padding: 6px;
	box-sizing: border-box;
	position: absolute;
	bottom: -185px;
	color: #fff;
	background: rgb(27, 27, 27, .5);
	transition: .5s;
}

.intro h3 {
	margin: 10px;
	font-weight: bold;
	font-size: 40px;
	text-align: center;
}

.intro p {
	margin: 20px;
	font-size: 20px;
	visibility: hidden;
	opacity: 0;

}

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

	.intro {
		bottom: -270px;
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

	.founder-container {
		grid-template-columns: 1fr;
	}

	.contenedor {
		margin: 0 10px;
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