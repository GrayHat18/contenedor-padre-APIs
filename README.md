# Contenedor Padre
Este proyecto es la carpeta contenedor principal de los microservicios rest que se agreguen como submodulos, el objetivo de este es ordenar y administrar 
las dependencias en común y su versión  que tengan 
diferentes APIs Rest y definir este proyecto como padre.

## Clonar y Configurar
Para clonar este repositorio, se debe crear una carpeta llamada "contenedor-padre" en un ruta segura del ambiente local, y luego ejecutar lo siguiente por línea de comandos:
```bash
git clone https://github.com/GrayHat18/contenedor-padre-APIs.git
cd contenedor-padre-APIs
git fetch
git pull origin master
```

# Estructura del Proyecto
Este proyecto solamente contiene un archivo pom.xml, el cual su configuración define que este es el parent de los microservicios rest que se agreguén como submodulos,
mediante lo siguiente:

```xml 
<parent>
 <groupId>org.springframework.boot</groupId> 
 <artifactId>spring-boot-starter-parent</artifactId>
 <version>3.2.3</version>
</parent>
```
Y la lista de submodulos actual es:
```xml
<modules>
 <module>apicriptografia-encriptacion</module>
 <module>apicriptografia-usuarios</module>
 <module>apigateway</module>
 <module>apicriptografia-usuarios-roles</module>
<modules>
```

# Arquitectura del Proyecto

![Arquitectura del Proyecto](https://private-user-images.githubusercontent.com/98406045/312212643-84aa23de-ae5c-400b-9765-037d7070c962.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTAyNzIxODAsIm5iZiI6MTcxMDI3MTg4MCwicGF0aCI6Ii85ODQwNjA0NS8zMTIyMTI2NDMtODRhYTIzZGUtYWU1Yy00MDBiLTk3NjUtMDM3ZDcwNzBjOTYyLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDAzMTIlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwMzEyVDE5MzEyMFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTZiY2IyNjNlODljMzgxNTI5MDA4ODY4NDA2YzVjYzNlOGJhYjBhZjY5ZTgwNTIwM2UwZGZkZGQ4NDY1MWRiY2ImWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.8GN9DpB1dMgSjNMX6IdNDsN6VEqVk9xPWv76cfqcE2E)
