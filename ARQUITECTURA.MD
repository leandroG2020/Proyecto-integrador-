Arquitectura del Sistema
1. Tipo de Arquitectura

Para este proyecto se utilizará una arquitectura Cliente – Servidor.

En este modelo los usuarios acceden al sistema desde una aplicación (cliente), mientras que el servidor se encarga de procesar las solicitudes, aplicar la lógica del sistema y almacenar la información en la base de datos.

Este tipo de arquitectura es común en aplicaciones web y permite que muchos usuarios puedan utilizar la plataforma al mismo tiempo.

2. Justificación de la Arquitectura

Se eligió esta arquitectura porque ofrece varias ventajas para el tipo de sistema que se desea construir:

Permite centralizar la información de los usuarios y los viajes

Facilita la gestión de la seguridad del sistema

Permite que muchos estudiantes utilicen la plataforma simultáneamente

Facilita el mantenimiento y la ampliación del sistema en el futuro

Además, es una arquitectura compatible con tecnologías modernas de desarrollo web.

3. Componentes del Sistema

El sistema estará compuesto por tres elementos principales.

Cliente

El cliente es la aplicación que utilizarán los estudiantes para interactuar con la plataforma.

Desde el cliente los usuarios podrán:

Registrarse en el sistema

Iniciar sesión

Publicar viajes

Buscar viajes disponibles

Solicitar unirse a un viaje

Ver sus viajes realizados

El cliente se desarrollará como una aplicación web.

Servidor

El servidor es el encargado de procesar las solicitudes enviadas por los clientes.

Entre sus funciones principales se encuentran:

Gestión de usuarios

Autenticación de estudiantes

Gestión de viajes

Gestión de solicitudes de pasajeros

Comunicación con la base de datos

El servidor será desarrollado utilizando Java con Spring Boot.

Base de Datos

La base de datos almacenará toda la información del sistema.

Algunos de los datos que se guardarán son:

Información de los usuarios

Viajes publicados

Solicitudes de pasajeros

Historial de viajes

Para este proyecto se utilizará MySQL.

4. Modelo de Capas

El servidor estará organizado utilizando un modelo de capas para facilitar la estructura del código.

Capa de Presentación

Se encarga de recibir las solicitudes que envían los usuarios desde la aplicación.

Aquí se encuentran los controladores de la API.

Capa de Lógica de Negocio

En esta capa se implementa el funcionamiento principal del sistema.

Por ejemplo:

Validar usuarios

Procesar solicitudes de viajes

Gestionar las rutas publicadas

Capa de Acceso a Datos

Esta capa se encarga de interactuar con la base de datos.

Incluye:

Repositorios

Consultas

Guardado y recuperación de información  

5. Flujo General del Sistema

El funcionamiento del sistema seguirá el siguiente proceso:

El estudiante ingresa a la plataforma.

El usuario inicia sesión en el sistema.

El estudiante puede crear un viaje o buscar uno disponible.

La aplicación envía la solicitud al servidor.

El servidor procesa la información.

Los datos se guardan en la base de datos.

El servidor envía la respuesta al cliente.
8. Seguridad

Para proteger la información del sistema se implementarán algunas medidas básicas de seguridad:

Registro e inicio de sesión de usuarios

Validación de correo institucional

Encriptación de contraseñas

Control de acceso a funcionalidades del sistema
