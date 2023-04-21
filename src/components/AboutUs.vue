<template>
<div class="container pt-2">
	<div class="row pt-5">
		<div class="col-sm-7 col-md-5">
			<img id="uno" src="https://smartdata.tonytemplates.com/electrician-v2/wp-content/uploads/2020/07/layout01-img01.jpg" alt="...">
			https://media.istockphoto.com/id/1268557129/es/foto/electricistas-cableado-de-una-nueva-construcci%C3%B3n.jpg?s=612x612&w=0&k=20&c=oSTD7KqJ_rccB7nPvJUQhxkoVpSa4SVJknGwyYrsNDE=
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
</template>

<script>
</script>

<style>
@import url('https://maxcdn.bootstrapcdn.com/font-awesome/4.5.0/css/font-awesome.min.css');

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
	height: 100%;
	top: 5%;
	padding: 10%;
	position: relative;
	background: #fff;
	font-family: 'Poppins', sans-serif;
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

</style>