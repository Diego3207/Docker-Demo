# Realizar un proyecto con Docker
Materia: Computación Tolerante a Fallas<br>
Maestro: MICHEL EMANUEL LOPEZ FRANCO<br>
Nombre: Diego Alonso Mercado Brizuela<br>
Carrera: Ingeniería en Computación<br>
Código: 215425636<br>
Fecha: 25/10/2023<br>
Sección: D06<br>
## Introducción
Docker es un proyecto de código abierto que automatiza el despliegue de aplicaciones dentro de contenedores de software, proporcionando una capa adicional de abstracción y automatización de virtualización de aplicaciones en múltiples sistemas operativos.
## Pruebas
### 1.- Instalar Docker
<br>
<img src="https://github.com/Diego3207/Docker-Demo/blob/main/Evidencia%201.png">
<br>
### 2.- Crear un archivo para probar el docker
<br>
En mi caso es un proyecto
<br>
### 3.- Crear un archivo (fuera de la carpeta creada anteriormente) llamado "Dockerfile" que tendrá lo siguiente:
<br>
/* es la imágen que vamos a instalar junto con la versión
FROM php:7.4.1-apache-buster
<br>
/*vamos a copiar la carpeta del ejemplo en la carpeta del Docker
COPY /Examen /var/www/html
<br>
/*exponemos el puerto 80 para ser accesado desde nuestra computadora
EXPOSE 80
<br>
<img src="https://github.com/Diego3207/Docker-Demo/blob/main/Evidencia%202.png">
<br>
### 4.- construimos la imágen, descargando apache, php, etc.
<br>
docker build -t hola-php .
<br>
### 5.- corremos la imágen que ya creamos
<br>
docker run -p 80:80 hola-php
<img src="https://github.com/Diego3207/Docker-Demo/blob/main/Evidencia%203.png">
# Conclusiones
Docker sirve muchísimo porque con esto podemos crear una máquina virtual con todas nuestras necesidades y hablo de dependencias, bibliotecas, etc. Entonces todo esto se lo pasamos a un compañero y literal ya no le da errores para compilar el mismo programa, con esto tenemos rendimiento para el proceso de trabajo porque la mayoría de este tipo de escenarios pasan errores y hay que estarlos resolviendo.
