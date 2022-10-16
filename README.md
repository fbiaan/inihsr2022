![HTR CLOUD INTEGRATION](documentation/images/prosegurlimpio.png)

# CORE API | HTR CLOUD INTEGRATION

## Proyecto
👋 Este Repositorio corresponde al equipo HTR CLOUD de PROSEGUR 👋
Descripcion : API for integration of RRHH core systems

## REQUISITOS 

### Requisitos de acceso

* Vpn conectada.
* Permisos de Git.


### Requisitos de compilacion 

Necesitas contar con Java 11 , lo puedes instalar ingresando a esta pagina de acuerdo al sistema opertivo usando este [instalador](https://www.oracle.com/java/technologies/downloads/#java11)

Otro requisito es Maven instalado ,  se puede descargar en este [link](https://maven.apache.org/download.cgi)

### Dependencias Principales
	org.springframework.cloud
	org.postgresql
	com.google.code.gson
	org.projectlombok
	
---

#### 👉❓ **Instalación de Lombok**

En caso de ser la primera vez que usas Lombok , es necesario realizar la instalación del mismo.

🔗 **🏳URL**: https://projectlombok.org/download

---




## Seguridad
![Seguridad](documentation/images/seguridad.jpg)


### Base de datos
Se necesita **registrar** la IP publica de la cual se va a acceder, ademas de las credenciales de acceso. Solicite al Proyect Lider este proceso.

### Vault🔒
Haciendo uso de Vault se ha conseguido sacar afuera del entorno de desarrollo el almacenamiento de secretos de nuestras aplicaciones.
El equipo de desarrollo solo necesita conocer la ruta de acceso para cada uno de los entornos en los que la aplicación sera desplegada.

Archivos 
*postgres
*HCM
*Meta4
Despliegues 
*Dev 
*Lab

| Archivos | Despliegues|
| ----- | -------------------------------------------- |
| Postgres| DEV|
| HCM     | LAB|
| Meta4    | |

Para entornos de desarrollo es necesario declarar la *variable de entorno* TOKEN_VAULT con un valor correcto para su autenticación , dicho valor es provisto por el Proyect Lider. 

### Depliegue e infraestructura
![despliegue](documentation/images/azuerkuber.jpg)

---
## Licencia
---