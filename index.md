<!DOCTYPE html>
<html>
<head>
	<meta charset="utf-8">
	<meta name="viewport" content="width=device width, initial-scale=1">
	<title>Configurateur de bineuse</title>
	<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css" integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous">
	<script src="https://code.jquery.com/jquery-3.2.1.slim.min.js" integrity="sha384-KJ3o2DKtIkvYIK3UENzmM7KCkRr/rE9/Qpg6aAZGJwFDMVNA/GpGFF93hXpG5KkN" crossorigin="anonymous"></script>
	<script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js" integrity="sha384-ApNbgh9B+Y1QKtv3Rn7W3mgPxhU9K/ScQsAP7hUibX39j7fakFPskvXusvfa0b4Q" crossorigin="anonymous"></script>
	<script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js" integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl" crossorigin="anonymous"></script>
	<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.0/jquery.min.js"></script>

	<style type="text/css">
		.choix {
		}

		.cargen{
			border-bottom: 1px dashed black;
			padding-bottom: 10px;
			margin-bottom: 10px;
			margin-top: 10px;
		}

		@font-face {
			font-family: ethnocentric_rg;
			src:url(font/ethnocentric_rg.ttf);
		}

		.textbig {
			font-weight: bold;
			margin-bottom: 1em;
			font-size: 1.5em;
			margin: 0.5em;
			font-family: ethnocentric_rg;
			background-color: #b3b3b3;
			text-align: center;
			border: 2px solid black;
			border-radius: 1em;
		}

		.texttitle {
			margin-bottom: 1em;
			font-size: 1.3em;
			font-style: italic;
			margin: 0;
			margin-bottom: 0.5em;
			font-family: ethnocentric_rg;
			color: #e53607;
			text-align: center;
		}

		.textres {
			font-weight: bold;
			font-size: 1.2em;
			text-align: center;
		}

		.textres2 {
			font-style: italic;
			font-size: 0.8em;
			text-align: center;
		}

		.imageres {
			width: 100px;
			transform: rotate(180deg);
		}

		.imageflag {
			width: 50px;
			height: 30px;
			margin-left: 1em;
			margin-right: 1em;
		}

		.buttonflag {
			border:0;
			background-color: white;
			cursor: pointer;
		}

		.selectlabel {
			padding: 0;
			font-weight: bold;
			margin-top: 10px;
			text-align: center;
			margin-bottom: 0;
		}

		.selectbox {
			margin-bottom: 2px;
			margin-left: 1em;
			margin-right: 1em;
			padding: 3px;
			padding-left: 15px;
			cursor: pointer;
			border-radius: 40px;
			background-color: #dddddd;
			color: black;
			font-weight: bold;
			border: 2px solid black;
		}
	</style>

</head>

<body>
	<div class="col mb-3">
		<div class="textbig" id="titre1">Configurateur de bineuse</div>
		<center>
			<button class="buttonflag">
				<img class="imageflag" id="flagfr" src="images/flag-fr.png">
			</button>
			<button class="buttonflag">
				<img class="imageflag" id="flages" src="images/flag-es.png">
			</button>
			<button class="buttonflag">
				<img class="imageflag" id="flagen" src="images/flag-en.png">
			</button>
		</center>
		<div class="texttitle" id="titre2">Caracteristiques generales</div>
		<div class="texttitle" id="nombin">BMIR 7 ou BSIR 7</div>
		<div class="row justify-content-center">
			<div class="col-5 col-sm-4 col-md-3 col-lg-2 my-auto mr-2">
				<div class="row choix">
					<label class="col-12 selectlabel" for="type" id="titre3">Type de bineuse</label>
					<select class="col selectbox" id="type" name="type">
						<option id="titre14">Fixe</option>
						<option id="titre15">Repliable</option>
					</select>
				</div>
				
				<div class="row choix">
					<label class="col-12 selectlabel" for="rang" id="titre4">Nombre de rangs</label>
					<select class="col selectbox" id="rang" name="rang">
						<option>4</option>
						<option>5</option>
						<option>6</option>
						<option>7</option>
						<option>8</option>
						<option>9</option>
						<option>10</option>
						<option>11</option>
						<option>12</option>
					</select>
				</div>
				
				<div class="row choix">
					<label class="col-12 selectlabel" for="ecart" id="titre5">Ecartement entre rangs</label>
					<select class="col selectbox" id="ecart" name="ecart">
						<option>450</option>
						<option>500</option>
						<option>550</option>
						<option>600</option>
						<option>700</option>
						<option>750</option>
						<option>800</option>
					</select>
				</div>

				<div class="row choix">
					<label class="col-12 selectlabel" for="coutre" id="titre6">Coutre de guidage</label>
					<select class="col selectbox" id="coutre" name="coutre">
						<option id="titre16">Sans</option>
						<option id="titre17">Avec</option>
					</select>
				</div>
			</div>
			<div class="col-4 my-auto ml-2">
				<div class="textres" id="titre7">Largeur de poutre</div>
				<div class="textres" id="largbin">4.2 m</div>
				<hr />
				<div class="textres" id="titre7b">Poids</div>
				<div class="textres" id="poidsbin">884 kg</div>
				<hr />
				<div class="textres" id="titre8">Prix de la bineuse*</div>
				<div class="textres" id="prixbin">13 855 €</div>
			</div>
		</div>
		<div class="textres2 cargen" id="attprix">Il ne s'agit que d'une estimation de prix, cela ne correspond en rien au prix définitif.</div>
		
		<div class="texttitle" id="titre9">Choix du module</div>
		<div class="row justify-content-center">
			<div class="col-5 col-sm-4 col-md-3 col-lg-2 mr-2">
				<div class="row choix">
					<label class="col-12 selectlabel" for="nbdent" id="titre10">Nombre de dents</label>
					<select class="col selectbox" id="nbdent" name="nbdent">
						<option value="20" id="titre18">3 (Rang <= 600)</option>
						<option value="10" id="titre19">5 (Rang > 600)</option>
					</select>
				</div>
				
				<div class="row choix">
					<label class="col-12 selectlabel" for="dent" id="titre11">Type de dents</label>
					<select class="col selectbox" id="dent" name="dent">
						<option value="0" id="titre20">32x10 patte d'oie</option>
						<option value="20" id="titre21">Soc scalpeur</option>
						<option value="40" id="titre22">Lame lelièvre</option>
					</select>
				</div>
				
				<div class="row choix">
					<label class="col-12 selectlabel" for="optav" id="titre12">Option avant</label>
					<select class="col selectbox" id="optav" name="optav">
						<option value="0"></option>
						<option id="pav" value="3">Protège plant</option>
						<option id="kav" value="6">Doigt Kress</option>
					</select>
				</div>
				
				<div class="row choix">
					<label class="col-12 selectlabel" for="optar" id="titre13">Option arrière</label>
					<select class="col selectbox" id="optar" name="optar">
						<option value="0"></option>
						<option value="2" id="titre23">Herse peigne</option>
						<option id="kar" value="1">Doigt Kress</option>
					</select>
				</div>
			</div>
			<div class="col-4 ml-2">
				
				<center><img class="imageres" id="image" src="images/m23.png"></center>
			</div>
		</div>
	</div>
</body>
</html>

<script>
	$(document).ready(function(){
		var nb = 0;
		var prixini = parseInt(13855);
		var milleprixini = parseInt(prixini / 1000);
		var centprixini = ("000" + (prixini - (milleprixini * 1000))).slice(-3);
		$('#rang').val(7);
		$('#prixbin').text(milleprixini + ' ' + centprixini + ' €');
		$('#ecart').val(500);
		$('#type').val('Repliable');
		$('#optav').val(3);
		$('select').on('change',function(){
			var poids = 0;
			var poidstot = 0;
			var prix = 0;
			var prixtot = 0;
			$('option').prop('disabled',false);
			var dent = parseInt($('#dent').val());
			var optav = parseInt($('#optav').val());
			var optar = parseInt($('#optar').val());
			var nbdent = parseInt($('#nbdent').val());
			var rang = parseInt($('#rang').val());
			var ecart = parseInt($('#ecart').val());
			var type = $('#type').val();
			var coutre = $('#coutre').val();
			if (dent == 40) {
				if (optav !== 0) {
					$('#optav').val(0);
					optav = 0;
				}
				$('#pav').prop('disabled',true);
				$('#kav').prop('disabled',true);
			} else if (optav == 6) {
				if (optar == 1) {
					$('#optar').val(0);
					optar = 0;
				}
				$('#kar').prop('disabled',true);
			}  else if (optar == 1) {
				if (optav == 6) {
					$('#optav').val(0);
					optav = 0;
				}
				$('#kav').prop('disabled',true);
			}
			nb = dent + optav + optar + nbdent;
			var image = 'images/m'+nb+'.png';
			$('#image').attr('src',image);

			if (nbdent == 10) {
				var nbd = 5;
				var dentmoins = 4;
				prix += 850;
				poids += 51.12;
				var poidsmoins = 5.37;
			} else {
				var nbd = 3;
				var dentmoins = 2;
				prix += 850;
				poids += 48.06;
				var poidsmoins = 2.31;
			}
			if (dent == 0) {
				prix += 116;
				if(nbd == 5){
					prix += 73;
				}
				poids += 3.4 * nbd;
				poidsmoins += 3.4 * dentmoins;
			} else if (dent == 20) {
				prix += 317;
				if(nbd == 5){
					prix += 202;
				}
				poids += 4.15 * nbd;
				poidsmoins += 4.15 * dentmoins;
			} else {
				if (nbd == 5) {
					prix += 548;
					poids += 22.01;
					poidsmoins += 17.86;
				} else {
					prix += 375;
					poids += 13.71;
					poidsmoins += 9.56;
				}
			}
			if (optav == 3){
				prix += 269;
				poids += 16.7;
				poidsmoins += 16.7;
			} else if (optav == 6) {
				prix += 799;
				poids += 17.15;
				poidsmoins += 17.15;
			}
			if (optar == 1) {
				prix += 924;
				poids += 22.2;
				poidsmoins += 22.2;
			} else if (optar == 2) {
				if (nbd == 5){
					prix += 462;
					poids += 9.03;
				} else {
					prix += 375;
					poids += 8.31;
				}
			}
			prix *= 100;
			prix = parseInt(prix);
			prix /= 100;
			poids *= 100;
			poids = parseInt(poids);
			poids /= 100;
			

			var larg = ecart * rang / 100;
			larg = parseInt(larg);
			larg += 2;
			larg /= 10;
			if (type == 'Fixe' || type == 'Fija' || type == 'Fixed') {
				var rampe = [3.5,4.2,5,6,6.6,7.4];
				for (var i = 0; i < rampe.length; i++) {
					if (larg <= rampe[i]) {
						larg = rampe[i];
						prixtot = 1130;
						i = rampe.length;
					}
				}
				poidstot = parseInt(80.86 + (24.22 * larg) + ((rang + 1) * poids) - poidsmoins);
			} else {
				var rampe = [4.2,5,6,6.6];
				for (var i = 0; i < rampe.length; i++) {
					if (larg <= rampe[i]) {
						larg = rampe[i];
						prixtot = 4000 + (11 * larg);
						i = rampe.length;
					}
				}
				poidstot = parseInt(368.92 - (24.22 * (6.6 - larg)) + ((rang + 1) * poids) - poidsmoins);
			}
			prixtot = parseInt(prixtot);
			if (coutre == "Avec" || coutre == 'Con' || coutre == 'With') {
				prixtot += 1221;
				poidstot += 96.36;
				poidstot = parseInt(poidstot);
			}
			prixtot += (rang + 1) * prix;
			prixtot = parseInt(prixtot);
			if(rang > 10){
				prixtot += 533;
			}
			prixtot = parseInt(prixtot);

			if (poidstot >= 1000){
				var mille = parseInt(poidstot/1000);
				var cent = ("000" + (poidstot - (mille * 1000))).slice(-3);
				$('#poidsbin').text(mille + ' ' + cent + ' kg');
			} else {
				$('#poidsbin').text(poidstot + ' kg');
			}

			$('#largbin').text(larg+' m');
			if (((type == 'Fixe' || type == 'Fija' || type == 'Fixed') && larg > 7.4) || ((type == 'Repliable' || type == 'Plegable' || type == 'Folding') && larg > 6.6)) {
				if (type == 'Fixe' || type == 'Repliable') {
					$('#prixbin').text('Nous consulter');
				}
				if (type == 'Fija' || type == 'Plegable') {
					$('#prixbin').text('Contáctenos');
				}
				if (type == 'Fixed' || type == 'Folding') {
					$('#prixbin').text('Contact us');
				}
			} else {
				if (prixtot >= 1000){
					var milleprixtot = parseInt(prixtot/1000);
					var centprixtot = ("000" + (prixtot - (milleprixtot * 1000))).slice(-3);
					$('#prixbin').text(milleprixtot + ' ' + centprixtot + ' €');
				} else {
					$('#prixbin').text(prixtot + ' €');
				}
			}

			if(ecart >= 600){
				if(type == 'Fixe'){
					$('#nombin').text('BLI ' + rang);
				} else {
					$('#nombin').text('BLIR ' + rang);
				}
			} else {
				if(type == 'Fixe'){
					$('#nombin').text('BMI ' + rang + ' ou BSI ' + rang);
				} else {
					$('#nombin').text('BMIR ' + rang + ' ou BSIR ' + rang);
				}
			}

		});
		$('#flagfr').on('click',function(){
			$('#titre1').text('Configurateur de bineuse');
			$('#titre2').text('Caracteristiques generales');
			$('#titre3').text('Type de bineuse');
			$('#titre4').text('Nombre de rangs');
			$('#titre5').text('Ecartement entre rangs');
			$('#titre6').text('Coutre de guidage');
			$('#titre7').text('Largeur de poutre');
			$('#titre7b').text('Poids');
			$('#titre8').text('Prix de la bineuse*');
			$('#titre9').text('Choix du module');
			$('#titre10').text('Nombre de dents');
			$('#titre11').text('Type de dents');
			$('#titre12').text('Option avant');
			$('#titre13').text('Option arrière');
			$('#titre14').text('Fixe');
			$('#titre15').text('Repliable');
			$('#titre16').text('Sans');
			$('#titre17').text('Avec');
			$('#titre18').text('3 (Rang <= 600)');
			$('#titre19').text('5 (Rang > 600)');
			$('#titre20').text("32x10 patte d'oie");
			$('#titre21').text('Soc scalpeur');
			$('#titre22').text('Lame lelièvre');
			$('#titre23').text('Herse peigne');
			$('#pav').text('Protège plant');
			$('#kav').text('Doigt Kress');
			$('#kar').text('Doigt Kress');
			var prixbin = $('#prixbin').text();
			if (prixbin == 'Contáctenos' || prixbin == 'Contact us') {
				$('#prixbin').text('Nous consulter');
			}
			$('#attprix').text("*Il ne s'agit que d'une estimation de prix, cela ne correspond en rien au prix définitif.");
		});
		$('#flages').on('click',function(){
			$('#titre1').text('Configurador de binadora');
			$('#titre2').text('Principales características');
			$('#titre3').text('Tipo de la binadora');
			$('#titre4').text('Número de filas');
			$('#titre5').text('Separación entre filas');
			$('#titre6').text('Cuchillas de guía');
			$('#titre7').text('Anchura de la viga');
			$('#titre7b').text('Peso');
			$('#titre8').text('Precio de la binadora*');
			$('#titre9').text('Selección de los módulos');
			$('#titre10').text('Número de brazos');
			$('#titre11').text('Tipo de brazos');
			$('#titre12').text('Opción delantera');
			$('#titre13').text('Opción trasera');
			$('#titre14').text('Fija');
			$('#titre15').text('Plegable');
			$('#titre16').text('Sin');
			$('#titre17').text('Con');
			$('#titre18').text('3 (Filas <= 600)');
			$('#titre19').text('5 (Filas > 600)');
			$('#titre20').text("32x10 pata de ganso");
			$('#titre21').text('Rejas tipo golondrina');
			$('#titre22').text('Láminas relieve');
			$('#titre23').text('Peine trasero');
			$('#pav').text('Protector de plantas');
			$('#kav').text('Dedos Kress');
			$('#kar').text('Dedos Kress');
			var prixbin = $('#prixbin').text();
			if (prixbin == 'Nous consulter' || prixbin == 'Contact us') {
				$('#prixbin').text('Contáctenos');
			}
			$('#attprix').text("*Esto es solo una estimación, no corresponde al precio final.");
		});
		$('#flagen').on('click',function(){
			$('#titre1').text('Cultivator configurator');
			$('#titre2').text('Main features');
			$('#titre3').text('Cultivator model');
			$('#titre4').text('Number of rows');
			$('#titre5').text('Inter row spacing');
			$('#titre6').text('Disc coulter');
			$('#titre7').text('Width');
			$('#titre7b').text('Weight');
			$('#titre8').text('Cultivator price*');
			$('#titre9').text('Unit selection');
			$('#titre10').text('Number of tines');
			$('#titre11').text('Type of tines');
			$('#titre12').text('Front option');
			$('#titre13').text('Back option');
			$('#titre14').text('Fixed');
			$('#titre15').text('Folding');
			$('#titre16').text('Without');
			$('#titre17').text('With');
			$('#titre18').text('3 (Rows <= 600)');
			$('#titre19').text('5 (Rows > 600)');
			$('#titre20').text("32x10 duckfoot");
			$('#titre21').text('Shovel');
			$('#titre22').text('Lelièvre blade');
			$('#titre23').text('Following harrow');
			$('#pav').text('Plant protection disc');
			$('#kav').text('Kress fingerweeder');
			$('#kar').text('Kress fingerweeder');
			var prixbin = $('#prixbin').text();
			if (prixbin == 'Contáctenos' || prixbin == 'Nous consulter') {
				$('#prixbin').text('Contact us');
			}
			$('#attprix').text("*This is only a price estimate, it does not correspond to the final price.");
		});
	});
</script>
