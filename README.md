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

