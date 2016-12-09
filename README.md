# Alan95
Sistema web 
<?php 
include("Menu1.php");
?>


<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">



	<link rel="stylesheet" type="text/css" href="css/bootstrap.min.css">
	<link rel="stylesheet" type="text/css" href="css/formulario-1.css">

	<link rel="stylesheet" href="//code.jquery.com/ui/1.12.1/themes/base/jquery-ui.css">
	<link href="https://fonts.googleapis.com/css?family=Baloo+Bhaina|Ramabhadra" rel="stylesheet">

	<script type="text/javascript" src="js/jquery-3.1.1.js"></script>
	
	<script src="https://code.jquery.com/ui/1.12.1/jquery-ui.js"></script>

	<script type="text/javascript" src="js/bootstrap.min.js"></script>
	

	<script>
		$(function(){
			$("#fechaingreso").datepicker({
				showOn: "focus",
				dateFormat: "dd-mm-yy",
				monthNamesShort: [ "Enero", "Febrero", "Marzo", "Abril", "Mayo", "Junio", "Julio", "Agosto", "Septimbre", "Octubre", "Noviembre", "Diciembre" ],
				dayNamesMin: [ 'D', 'L', 'M', 'M', 'J', 'V', 'S'],
				changeMonth:true,
				changeYear:true,
				showButtonPanel:true,
				 buttonText: "Ingreso",
				 currentText: "Hoy",
				 closeText: "Cerrar",
			});
			$("#fechamensualidad").datepicker({
				dateFormat: "dd-mm-yy",
				monthNamesShort: [ "Enero", "Febrero", "Marzo", "Abril", "Mayo", "Junio", "Julio", "Agosto", "Septimbre", "Octubre", "Noviembre", "Diciembre" ],
				dayNamesMin: [ 'D', 'L', 'M', 'M', 'J', 'V', 'S'],
				changeMonth:true,
				changeYear:true,
				showButtonPanel:true,
				 buttonText: "Mensualidad",
				 currentText: "Hoy",
				 closeText: "Cerrar",
			});
			$("#fechainicio").datepicker({
				dateFormat: "dd-mm-yy",
				monthNamesShort: [ "Enero", "Febrero", "Marzo", "Abril", "Mayo", "Junio", "Julio", "Agosto", "Septimbre", "Octubre", "Noviembre", "Diciembre" ],
				dayNamesMin: [ 'D', 'L', 'M', 'M', 'J', 'V', 'S'],
				changeMonth:true,
				changeYear:true,
				showButtonPanel:true,
				 buttonText: "Mensualidad",
				 currentText: "Hoy",
				 closeText: "Cerrar",
			});
		});
		
	</script>

	<title>Formulario de Clientes</title>
	
</head>
<body class="cuerpofor">
<form action="" class="form1" method="POST">
	
	<div class="col-md-7">
		
			
			<fieldset>
			<legend class="leyenda">Datos-Generales:</legend>
				<div class="row">

						<div class="col-md-6">
						    <div class="form-group">
    							<label class="col-sm-2 control-label " id="labelclave">Clave:</label> 
	    						<div class="col-sm-3">
	     							<input type="text" class="form-control input-sm" id="clave" placeholder="Clave" 
	     							disabled="">	     							
	    						</div>

		    					<div class="col-md-1">
							    	<button class="btn btn-primary">...</button>
							    </div>
						    </div>
						</div>

						<div class="col-md-6">
							<div class="form-group">
								<label class="col-sm-3 control-label" id="labelclave">Nombre:</label>
								<div class="col-sm-8">
									<input id="nombre" name="nombre" type="text" class="form-control input-sm"  placeholder="Nombre Completo" required=""></input>
								</div>	
							</div>
						</div>

						<div class="col-md-6">
						    <div class="form-group">
    							<label class="col-sm-2 control-label" id="labelclave">Edad:</label>
	    						<div class="col-sm-5">
	     							<input id="edad" name="edad" type="text" class="form-control input-sm"  placeholder="Edad" required="">
	    						</div>
						    </div>
						</div>

						<div class="col-md-6">
							<div class="form-group">
								<label class="col-sm-3 control-label" id="labelclave">Celular:</label>
								<div class="col-sm-8">
									<input id="celular" name="celular" type="text" class="form-control input-sm"  placeholder="Celular" required=""></input>
								</div>	
							</div>
						</div>

						<div class="col-md-6 form-group-sm">
						    <div class="form-group">
    							<label class="col-sm-3 control-label" id="labelclave">Estatura:</label>
	    						<div class="col-sm-5">
	     							<input id="estatura" name="estatura" type="text" class="form-control"  placeholder="Estatura" required="">
	    						</div>
						    </div>
						</div>

						<div class="col-md-6 form-group-sm">
							<div class="form-group">
								<label class="col-sm-3 control-label" id="labelclave">Dirección:</label>
								<div class="col-sm-8">
									<input id="direccion" name="direccion" type="text" class="form-control" placeholder="Dirección Completo" required=""></input>
								</div>	
							</div>
						</div>

						<div class="col-md-6 form-group-sm">
						    <div class="form-group">
    							<label class="col-sm-3 control-label" id="labelclave">Fecha:</label>
	    						<div class="col-sm-5">
	     							<input id="fechaingreso" name="fechaingreso" type="text" class="form-control"  placeholder="Fecha de Ingreso" required="">
	    						</div>
						    </div>
						</div>

						<div class="col-md-6 form-group-sm">
							<div class="form-group">
								<label class="col-sm-3 control-label" id="labelclave">Fecha:</label>
								<div class="col-sm-6">
									<input id="fechamensualidad" type="text" class="form-control"  placeholder="Fecha de Mensualidad" required="" ></input>
								</div>	
							</div>
						</div>

						<div class="col-md-6 form-group-sm">
						    <div class="form-group">
    							<label class="col-sm-3 control-label" id="labelclave">Disciplina:</label>
	    						<div class="col-sm-5">
	     							<select id="disciplina" name="" class="form-control" required="">
									  <option>Disciplinas...</option>
									  <option>Spinning</option>
									  <option>Abdominales</option>
									  <option>Circuit</option>
									  <option>Zumba</option>
									</select>
	    						</div>
						    </div>
						</div>

						<div class="col-md-6 form-group-sm">
							<div class="form-group">
								<label class="col-sm-2 control-label id=" id="labelclave">Cupo:</label>
								<div class="col-sm-3">
									<input id="cupo" name="cupo" type="text" class="form-control"  placeholder="Cupo" required=""></input>
								</div>	
							</div>
						</div>	
				</div>
			</fieldset>	

<!-- parte inicial del grupo de los botones -->			
				<legend></legend>
				<div class="container col-md-10">

					<input id="btn-guardar" type="button" class="btn btn-primary" value="Guardar"></input>	
							
					<input id="btn-actualizar" type="button" class="btn btn-success" value="Actualizar"></input>
							
					<button type="submit" class="btn btn-danger">Eliminar</button>

					<button type="button" class="btn btn-primary" data-toggle="modal" data-target="#exampleModal" data-whatever="@mdo">Modal</button>

				<span id="result"></span>

<script type="text/javascript">

$('#exampleModal').on('show.bs.modal', function (event) {
  var button = $(event.relatedTarget) // Button that triggered the modal
  var recipient = button.data('whatever') // Extract info from data-* attributes
  // If necessary, you could initiate an AJAX request here (and then do the updating in a callback).
  // Update the modal's content. We'll use jQuery here, but you could use a data binding library or other methods instead.
  var modal = $(this)
  modal.find('.modal-title').text('New message to ' + recipient)
  modal.find('.modal-body input').val(recipient)
})

</script>

				</div>	

					

	</div>
<!-- PARTE FINAL DE PRIMER CONTENEDOR -->


<!-- PARTE INICIAL DEL SEGUNDO CONTENEDOR -->
<div class="modal fade" id="exampleModal" tabindex="-1" role="dialog" aria-labelledby="exampleModalLabel">
  <div class="modal-dialog" role="document">
    <div class="modal-content">

      <div class="modal-header">
        <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
        <h4 class="modal-title" id="gridSystemModalLabel">DATOS CORPORALES INICIALES</h4>
      </div>

<div class="modal-body">
<form>
				<div class="row">
						<div class="col-md-6">
						    <div class="form-group has-success has-feedback">
    							<label class="col-md-3 control-label " id="labelclave">Clave:</label>
	    						<div class="col-sm-5">
	     							<input type="text" class="form-control input-sm" id="clave" placeholder="Clave" 
	     							disabled="">
	    						</div>
						    </div>
						</div>
				</div>
				<div class="row">
						<div class="col-md-6 form-group-sm">
						    <div class="form-group">
    							<label class="col-sm-3 control-label" id="labelclave">Fecha:</label>
	    						<div class="col-sm-7">
	     							<input id="fechainicio" name="fechainicio" type="text" class="form-control"  placeholder="Fecha de Inicio" required="">
	    						</div>
						    </div>
						</div>
				</div>

			<div class="row">
				<div class="col-md-6 form-group-sm">
					<div class="form-group">
						<label class="col-md-3 control-label id=" id="labelclave">Peso:</label>			
						<div class="col-sm-7">
							<input id="peso" name="peso" type="text" class="form-control" id="cupo1" placeholder="Peso Nuevo" required=""></input>
						</div>	
					</div>
				</div>	
			</div>

			<div class="row">
				<div class="col-md-6 form-group-sm">
					<div class="form-group">
						<label class="col-md-3 control-label id=" id="labelclave">Medida:</label>
						<div class="col-sm-7">
							<input id="medidapierna" name="medidapierna" type="text" class="form-control" placeholder="Medida-Pierna" required=""></input>
						</div>	
					</div>
				</div>
			</div>

			<div class="row">
				<div class="col-md-6 form-group-sm">
					<div class="form-group">
						<label class="col-sm-3 control-label id=" id="labelclave">Medida:</label>			
						<div class="col-sm-7">
							<input id="medidacintura" name="medidacintura" type="text" class="form-control"  placeholder="Medida-Cintura" required=""></input>
						</div>	
					</div>
				</div>
			</div>

			<div class="row">
				<div class="col-md-6 form-group-sm">
					<div class="form-group">
						<label class="col-sm-6 control-label id=" id="labelclave">Observaciones:</label>			
						<div class="col-sm-7">
							<textarea id="observaciones" name="observaciones" class="form-control" rows="3" placeholder="Escriba las Observaciones del cliente" required=""></textarea>
						</div>	
					</div>
				</div>
			</div>
</form>
 </div>
      <div class="modal-footer">
        <button type="button" class="btn btn-default" data-dismiss="modal">Cerrar</button>
        <button type="button" class="btn btn-primary">Guardar</button>
      </div>

    </div><!-- /.modal-content -->
  </div><!-- /.modal-dialog -->
</div><!-- /.modal -->
<!-- PARTE FINAL DEL SEGUNO CONTENEDORS -->


<!-- Parte del label de buscar -->
<legend></legend>
		<div class="col-xs-3">
				<input type="text" class="form-control input-sm" id="" placeholder="Buscar...">
		</div>
<!-- PARTE FINAL DEL LABEL BUSCAR-->


<!-- PARTE DE LA TABLA -->	
<section class="container col-md-12">
	
	<div class="row">
	<div class="col-md-12">
		<div class="panel panel-primary">
			
			<div class="panel-heading">
				<h3 class="panel-title h3cab">Tabla de Todos los Clientes</h3>
			</div>

			<div class="panel-body">
				<div class="table-responsive">
					<table class="table table-hover">
						<tr>
							<th width="150">Nombre</th>
							<th width="30">Celular</th>
							<th width="20">Edad</th>
							<th width="50">Estatura</th>
							<th width="150">Direccion</th>
							<th width="150">Fecha-Ingreso</th>
							<th width="150">Fecha-Mensualidad</th>
							<th width="90">Disciplina</th>
							<th width="50"> OPTIONES</th>
						</tr>
						<?php
								
							$conexion=mysqli_connect("localhost", "root", "alan95", "sportcenterx");

							$sql="SELECT * FROM cliente ORDER BY Id_Cliente ASC";
							$resultado = mysqli_query($conexion, $sql);
								
								while ($registro2 = mysqli_fetch_array($resultado)) {
									echo '
										<tr>
											<td>'.$registro2['Nombre_Completo'].'</td>
											<td>'.$registro2['Celular'].'</td>
											<td>'.$registro2['Edad'].'</td>
											<td>'.$registro2['Estatura'].'</td>
											<td>'.$registro2['Direccion'].'</td>
											<td>'.$registro2['Fecha_Ingreso'].'</td>
											<td>'.$registro2['Fecha_Mensualidad'].'</td>
											<td>'.$registro2['Disciplina'].'</td>
											<td>
												<button><a href="javascript:eliminarclase('.$registro2['Id_Cliente'].');" class="glyphicon glyphicon-remove-circle"></a></button>
												<button id="btneditar"><a href="javascript:editarclase('.$registro2['Id_Cliente'].');" class="glyphicon glyphicon-edit"></a></button>
											</td>

										</tr>
									';
								}
							?>
					</table>
			</div>
			</div>

		</div>

	</div>
	</div>

</section>
<!-- PARTE FINAL DE LA TABLA -->

</form>
</body>
</html>

<script type="text/javascript">

$(document).ready(function(){
	
		$('#btn-guardar').click(function(){
			var nombre = $('#nombre').val;
			var edad = $('#edad').val();
			var celular = $('#celular').val();
			var estatura = $('#estatura').val();
			var direccion = $('#direccion').val();
			var fechaingreso = $('#fechaingreso').val();
			var fechamensualidad = $('#fechamensualidad').val();
			var disciplina = $('#disciplina').val();

			alert(nombre);
			alert(edad);
			alert(celular);
			alert(estatura);
			alert(direccion);
			alert(fechaingreso);
			alert(fechamensualidad);
			alert(disciplina);


			var url = "php/GuardarCliente.php";
			alert(url);

			
			var total = nombre.length * edad.length * celular.length * estatura.length * direccion.length * fechaingreso.length * fechamensualidad.length* disciplina.length;

			alert(total);

			if (total>0) {

				$.ajax({
					url:url,
					method:"POST",
					data:{nombre:nombre, edad:edad, celular:celular, estatura:estatura, direccion:direccion, fechaingreso:fechaingreso, fechamensualidad:fechamensualidad, disciplina:disciplina},
					cache:false,

					beforeSend:function(){
						console.log("enviando los datos a la base de datos ");
					},
					success:function(data){
						console.log("data");	

						$("#result").html("<div class='alert alert-dismissible alert-success'><button type='button' class='close' data-dismiss='alert'>&times;</button><strong></strong>Los Datos Fueron Guardar Exitosamente</div>").show(300).delay(4000).hide(300);	
						document.location.href = 'http://localhost/SportCenter1/formulario-1.php';
					},
				});
			}else{
				$("#result").html("<div class='alert alert-dismissible alert-danger'><button type='button' class='close' data-dismiss='alert'>&times;</button><strong>¡ERROR!</strong> Los campos estan vasios</div>").show(300).delay(3000).hide(300);
			}
		});
	});	
</script>


/////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
GuardarCliente.php

<?php

$conexion=mysqli_connect("localhost", "root", "alan95", "sportcenterx");

if(isset($_POST["nombre"]) && isset($_POST["edad"]) && isset($_POST["celular"]) && isset($_POST["estatura"]) && isset($_POST["direccion"]) && isset($_POST["fechaingreso"]) && isset($_POST["fechamensualidad"]) && isset($_POST["disciplina"])){

	$nombre = mysqli_real_escape_string($conexion, $_POST["nombre"]);
	$edad =mysqli_real_escape_string($conexion, $_POST["edad"]);
	$celular =mysqli_real_escape_string($conexion, $_POST["celular"]);
	$estatura =mysqli_real_escape_string($conexion, $_POST["estatura"]);
	$direccion =mysqli_real_escape_string($conexion, $_POST["direccion"]);
	$fechaingreso =mysqli_real_escape_string($conexion, $_POST["fechaingreso"]);
	$fechamensualidad =mysqli_real_escape_string($conexion, $_POST["fechamensualidad"]);
	$disciplina =mysqli_real_escape_string($conexion, $_POST["disciplina"]);

//peticiones a la base de datos.
	$sql1="INSERT INTO cliente (Nombre_Completo, Celular, Edad, Estatura, Direccion, Fecha_Ingreso, Fecha_Mensualidad, Disciplina) VALUES ('".$nombre."', '".$celular."', '".$edad."', '".$estatura."', '".$direccion."', '".$fechaingreso."', '".$fechamensualidad."', '".$disciplina."')";

			$resultado = mysqli_query($conexion, $sql1);
			$numero = mysqli_num_rows($resultado);

			if($numero > 0){
				$data = mysqli_fetch_array($resultado);
				$_SESSION["Usuario"] = $data["Usuario"];
				echo $data["Usuario"];
			}
}
?>






