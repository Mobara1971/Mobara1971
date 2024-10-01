<!DOCTYPE html>
<html lang="fr">
<head>
<title>doc</title>
</head>
<body>
	<form>
		<fieldset>
			<legend>Genre</legend>
			<label>Sexe :</label>
			<br>
			<input type="radio" id="M" name="sexe" value="M" onclick="afficherMessage(this)"> M
			<input type="radio" id="F" name="sexe" value="F" onclick="afficherMessage(this)"> F
			<br>
			<p id="message"></p>
			<input type="submit" id="envoyer" value="Envoyer" onclick="monsexe()">
		</fieldset>
	</form>

	<script>
		function afficherMessage(sexe) {
			var message = document.getElementById('message');
			
		}

		function monsexe() {
			var sexeM = document.getElementById('M');
			var sexeF = document.getElementById('F');
			var message = document.getElementById('message');

			if (sexeM.checked) {
				alert('vous etes de sexe masculin');
			} else if (sexeF.checked) {
				alert('vous etes de sexe féminin');
			} else {
				alert('Veuillez sélectionner votre sexe');
			}
		}
	</script>
</body>
</html>
