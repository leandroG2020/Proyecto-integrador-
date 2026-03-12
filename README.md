# Proyecto-integrador-
Este repositorio contendra el proyecto integrador como aplicacion para los estudiantes de la universidad luis amigo para transportarse (mini-uber)

# Arquitectura del Sistema

## 1. Tipo de Arquitectura

El sistema utilizará una **Arquitectura Cliente–Servidor**, la cual permite que múltiples usuarios (clientes) se conecten a un servidor central que gestiona la información, lógica del sistema y seguridad.

Este modelo es ampliamente utilizado en aplicaciones web y móviles, especialmente en plataformas de transporte como Uber o DiDi.

En este proyecto, los estudiantes de la Universidad Católica Luis Amigó utilizarán una aplicación web o móvil (cliente) para interactuar con el sistema, mientras que el servidor central administrará los usuarios, viajes y solicitudes.

---

# 2. Justificación de la Arquitectura

La arquitectura Cliente–Servidor es adecuada para este proyecto porque:

- Permite centralizar la información de usuarios y viajes.
- Facilita la autenticación y control de seguridad.
- Permite que múltiples estudiantes utilicen la plataforma simultáneamente.
- Facilita la escalabilidad del sistema en el futuro.

Además, esta arquitectura es compatible con tecnologías modernas de desarrollo web y backend en Java.

---

# 3. Componentes de la Arquitectura

## Cliente

El cliente corresponde a la interfaz que utilizarán los estudiantes para interactuar con el sistema.

Funciones principales:

- Registro de usuarios
- Inicio de sesión
- Crear rutas o viajes
- Buscar viajes disponibles
- Solicitar unirse a un viaje
- Ver historial de viajes

El cliente puede implementarse como:

- Aplicación web
- Aplicación móvil

---

## Servidor

El servidor es el encargado de procesar las solicitudes de los clientes y gestionar la lógica del sistema.

Funciones del servidor:

- Gestión de usuarios
- Autenticación
- Gestión de viajes
- Gestión de solicitudes de pasajeros
- Almacenamiento de datos
- Control de seguridad

El servidor estará desarrollado utilizando **Java y Spring Boot**.

---

# 4. Modelo de Capas

Dentro del servidor se utilizará un modelo por capas para organizar el código.

## Capa de Presentación

Se encarga de recibir las solicitudes del cliente.

Ejemplo:

- API REST
- Controladores

---

## Capa de Lógica de Negocio

Contiene la lógica principal del sistema.

Ejemplo:

- Gestión de viajes
- Validación de usuarios
- Procesamiento de solicitudes

---

## Capa de Acceso a Datos

Se encarga de interactuar con la base de datos.

Ejemplo:

- Repositorios
- Consultas a la base de datos

---

# 5. Flujo del Sistema

1. Un estudiante abre la aplicación.
2. El estudiante inicia sesión.
3. El usuario crea un viaje o busca uno disponible.
4. El cliente envía la solicitud al servidor.
5. El servidor procesa la información.
6. El servidor guarda los datos en la base de datos.
7. El sistema devuelve la respuesta al cliente.

---

# 6. Diagrama Conceptual de Arquitectura

Cliente (Web o App)

↓

API REST (Spring Boot)

↓

Lógica de negocio

↓

Base de datos

---

# 7. Stack Tecnológico

El sistema será desarrollado utilizando el siguiente stack tecnológico:

## Backend

- Java
- Spring Boot
- Spring Security
- Maven

## Base de Datos

- MySQL o PostgreSQL

## Frontend

- HTML
- CSS
- JavaScript
- React (opcional)

## Control de Versiones

- Git
- GitHub

---

# 8. Seguridad

Para garantizar la seguridad del sistema se implementarán:

- Autenticación de usuarios
- Validación de correo institucional
- Encriptación de contraseñas
- Control de acceso

---

# 9. Escalabilidad

La arquitectura Cliente–Servidor permite:

- Agregar más usuarios sin afectar el sistema.
- Integrar nuevas funcionalidades en el futuro.
- Escalar el backend si la plataforma crece.

  # Plataforma de Transporte Compartido Universitario

## Descripción del Proyecto

Este proyecto consiste en el desarrollo de una plataforma digital que permita a los estudiantes de la Universidad Católica Luis Amigó compartir transporte entre ellos de forma segura, económica y organizada.

La aplicación permitirá que los estudiantes publiquen rutas, encuentren compañeros de viaje y reduzcan los costos de transporte.

---

# Problema

Actualmente muchos estudiantes enfrentan dificultades para movilizarse hacia y desde la universidad debido a:

- Falta de vehículo propio
- Transporte público congestionado
- Altos costos de servicios como Uber o DiDi
- Falta de coordinación entre estudiantes para compartir transporte

Esto genera gastos innecesarios y problemas de seguridad.

---

# Solución

La solución propuesta es una **plataforma digital de transporte compartido entre estudiantes**, donde los usuarios puedan:

- Publicar rutas
- Buscar viajes disponibles
- Compartir gastos de transporte
- Viajar con estudiantes verificados de la universidad

---

# Impacto

Este sistema permitirá:

- Reducir costos de transporte
- Mejorar la seguridad de los estudiantes
- Optimizar la movilidad universitaria
- Reducir la congestión de transporte

---

# Proyección

A futuro el sistema podría:

- Integrarse con aplicaciones móviles
- Incluir sistema de calificación de usuarios
- Implementar notificaciones en tiempo real
- Ampliarse a otras universidades

---

# Tecnologías Utilizadas

Backend:

- Java
- Spring Boot

Frontend:

- HTML
- CSS
- JavaScript

Base de Datos:

- MySQL

Control de versiones:

- Git
- GitHub

---

# Arquitectura

El sistema está basado en una **Arquitectura Cliente–Servidor**, donde los estudiantes utilizan una aplicación cliente que se conecta a un servidor central que gestiona los usuarios y los viajes.

Más detalles disponibles en el archivo **ARQUITECTURA.md**.
