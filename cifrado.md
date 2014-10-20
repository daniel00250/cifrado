<html lang="es">
<head>
	<meta charset="UTF-8">
	<title>Deisy Peña</title>
	<scrip>
	var Palabra
	nom_div("Codificar").addEventListener("click", function() 
	{
		Palabra = nom_div("Codificacion").value; 
		
		Palabra = Palabra.toUpperCase();

		var Resultado = [];

		for(var i = 0; i < Palabra.length; i++) //recorre cada letra    
		{

			if(Palabra[i] == "A"){ Resultado[i] = "Z"}
			if(Palabra[i] == "B"){ Resultado[i] = "Y"}
			if(Palabra[i] == "C"){ Resultado[i] = "X"}
			if(Palabra[i] == "D"){ Resultado[i] = "W"}
			if(Palabra[i] == "E"){ Resultado[i] = "V"}
			if(Palabra[i] == "F"){ Resultado[i] = "U"}
			if(Palabra[i] == "G"){ Resultado[i] = "T"}
			if(Palabra[i] == "H"){ Resultado[i] = "S"}
			if(Palabra[i] == "I"){ Resultado[i] = "R"}
			if(Palabra[i] == "J"){ Resultado[i] = "Q"}
			if(Palabra[i] == "K"){ Resultado[i] = "P"}
			if(Palabra[i] == "L"){ Resultado[i] = "O"}
			if(Palabra[i] == "M"){ Resultado[i] = "N"}
			if(Palabra[i] == "N"){ Resultado[i] = "M"}
			if(Palabra[i] == "O"){ Resultado[i] = "L"}
			if(Palabra[i] == "P"){ Resultado[i] = "K"}
			if(Palabra[i] == "Q"){ Resultado[i] = "J"}
			if(Palabra[i] == "R"){ Resultado[i] = "I"}
			if(Palabra[i] == "S"){ Resultado[i] = "H"}
			if(Palabra[i] == "T"){ Resultado[i] = "G"}
			if(Palabra[i] == "U"){ Resultado[i] = "F"}
			if(Palabra[i] == "V"){ Resultado[i] = "E"}
			if(Palabra[i] == "W"){ Resultado[i] = "D"}
			if(Palabra[i] == "X"){ Resultado[i] = "C"}
			if(Palabra[i] == "Y"){ Resultado[i] = "B"}
			if(Palabra[i] == "Z"){ Resultado[i] = "A"}
			if(Palabra[i] == " "){ Resultado[i] = " "}	//si encuentra un espacio lo deja tal y como estaba 		
		}

		Resultado = Resultado.join(""); //Quita las "," y une las palabras
		nom_div("Producto").value = Resultado;
	});

	function nom_div(div)
	{
		return document.getElementById(div);
	}
}
</scrip>
	
</head>
<body>
	<center>
		<div id = "cuerpo">
			<h1>
				daniel camilo ramirez</br>
				
			</h1>

			<input type="text" id="Codificacion" placeholder = "Ingrese palabra a codificar"><br>
			<input type="button" id="Codificar" value="Codifica!"><br>
			<input type="text" id="Producto"></div>
			
		</div>
	</center>	
</body>
</html>
