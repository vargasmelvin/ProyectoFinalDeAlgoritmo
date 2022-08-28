Algoritmo  renta
	//requisitos
	Escribir "MELVIN SMERLIN VARGAS SMITH (21-MIEN-1-011) (0435)";
	//entrada
	Definir contador Como Entero;
	Definir ModalidadV Como Entero;
	Definir Nombre1 Como Caracter;
	Definir Vehiculo1 Como Entero;
	Definir Seguro1 Como Entero;
	Definir Accesorio1 Como Entero;
	Definir Precio Como Entero;
	Definir cerrar Como Caracter;
	Precio=0;
	contador=0;
	//Proceso 
	
	
	Escribir "Muy bienvenido a Oneday rent a car  :)";
	Escribir "Si el cliente prefiere obtener el vehiculo ahora mismo ingrese 1, Si prefiere agendar una cita  ingrese 2";
	Leer ModalidadV;
	Si ModalidadV = 1 Entonces
		Escribir "Vemos que prefiere obtener su vehiculo ahora mismo";
	SiNo
		Escribir "Vemos que prefiere agendar una cita";	
	Fin Si
	Mientras contador < 1 Hacer
		Escribir "ingrese el nombre del cliente";
		Leer  Nombre1;
		Escribir "Decision del cliente";
		Escribir "Vehiculo";
		Escribir "1 Toyota Corrolla, 2 Hyundai Sonata, 3 Nissan V13";
		Leer Vehiculo1;
		Escribir "Seguro";
		Escribir "1 Con seguro, 2 Sin seguro";
		Leer Seguro1;
		Escribir "Accesorio";
		Escribir "1 Vidrio polarizado, 2 Vidrio no polarizado";
		Leer Accesorio1;
	
		Si Vehiculo1 = 1 Entonces
			Escribir "El cliente: ", Nombre1 " " , " " , "Alquilo un Toyota Corrolla";
			Precio = Precio+2000;
		SiNo
			si Vehiculo1 = 2 Entonces
				Escribir "El cliente: ", Nombre1 " " , " " , "Alquilo un Hyundai Sonata";
				Precio = Precio+3000;
			SiNo
				Escribir "El cliente: ", Nombre1 " " , " " , "Alquilo un Nissan V13";
				Precio = Precio+1000;
			FinSi
		FinSi
		contador = contador+1;
		si Seguro1 = 1 Entonces
			Escribir "El cliente: ", Nombre1 " " , " " , "tendra su vehiculo asegurado";
			Precio = Precio+5000
		SiNo
			Escribir "El cliente: ", Nombre1 " " , " " , "no tendra su vehiculo asegurado";
			Precio = Precio+0
		FinSi
	si Accesorio1 = 1 Entonces
		Escribir "El cliente: ", Nombre1 " " , " " , "tendra el vidrio de su vehiculo polarizado";
		Precio = Precio+4000
	SiNo
		Escribir "El cliente: ", Nombre1 " " , " " , "no tendra el vidrio de su vehiculo polarizado";
		Precio = Precio+0
	FinSi
	Escribir "Haga Enter si desea continuar con su alquiler del vehiculo";
	Leer cerrar;
	//salida
	
	
	Limpiar Pantalla;
	Escribir 		"/////" "Renta de vehiculos Vargas" "///////" "Factura" "///////";
	Escribir 	" ";
	Escribir "Fecha: 27/08/2022";
	Escribir "Nombre: " Nombre1;
	si Vehiculo1 = 1 Entonces
		Escribir "Alquilo un Toyota Corrolla por 2000 pesos";
	SiNo
		si Vehiculo1 = 2 Entonces
			Escribir "Alquilo un Hyundai Sonata por 3000 pesos";
		SiNo
				Escribir "Alquilo un Nissan V13 por 1000 pesos";
			FinSi
		FinSi
	si Seguro1 = 1 Entonces
		Escribir "Vehiculo asegurado 5000 pesos"
	SiNo
			Escribir "Vehiculo no asegurado 0 pesos"
		FinSi
		si Accesorio1 = 1 Entonces
			Escribir "Su vehiculo posee vidrios polarizados 4000 pesos"
		SiNo
			Escribir "Su vehiculo no posee vidrios polarizados 0 pesos"
		FinSi
		Escribir "El Precio total es de:", Precio " " "pesos";
	FinMientras
	
FinAlgoritmo
