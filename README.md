Importación de la imagen (equipo destino)
Una vez ubicado el archivo .tar en el equipo destino, se procede a importarlo con:
docker load -i nombre_imagen.tar
Este proceso reconstruye la imagen en el sistema local.

Verificación de la imagen
Para comprobar que la imagen fue importada correctamente:
docker images
Se debe visualizar la imagen con su nombre y etiqueta correspondiente.

Ejecución del contenedor
Para ejecutar un contenedor a partir de la imagen importada:
docker run -d -p 8080:80 nombre_imagen:tag
Este comando inicia el contenedor en segundo plano y realiza el mapeo de puertos.

Uso de Docker Desktop
Desde la interfaz gráfica de Docker Desktop:
•	Acceder a la sección Images 
•	Verificar la imagen importada 
•	Seleccionar la opción Run 
•	Configurar parámetros como puertos y variables de entorno 
•	Ejecutar el contenedor 
