PRACTICA Nª 1 
UNIV: ROSA KATERINE GONZALES CHOQUE 
CI: 8295762

📚 Universidad API

API REST para la gestión de estudiantes en una universidad, desarrollada con Spring Boot.

🚀 Características

CRUD de estudiantes (Crear, Leer, Actualizar, Eliminar).

Uso de DTOs para transferencia de datos.

Implementación de servicios y repositorios con inyección de dependencias.

Respuestas HTTP estándar.

📦 Tecnologías

Java 17

Spring Boot

Spring Web

Spring Data

Jakarta Annotations

📂 Estructura del Proyecto

├── src/main/java/com/universidad
│   ├── controller
│   ├── dto
│   ├── model
│   ├── repository
│   ├── service
│   ├── service/impl
│   ├── UniversidadApplication.java
├── src/main/resources
│   ├── application.properties
├── pom.xml
└── README.md

🛠 Instalación y Ejecución

1️⃣ Clonar el repositorio

git clone https://github.com/KatRose7/RegistroUniversitario.git
cd RegistroUniversitario

2️⃣ Construir y ejecutar el proyecto

mvn spring-boot:run

🔥 Endpoints

📌 Obtener todos los estudiantes

GET /api/estudiantes

📌 Obtener un estudiante por ID

GET /api/estudiantes/{id}

📌 Crear un estudiante

POST /api/estudiantes

Cuerpo JSON:

{
  "nombre": "Juan",
  "apellido": "Pérez",
  "email": "juan.perez@example.com",
  "fechaNacimiento": "2000-05-15",
  "numeroInscripcion": "S001"
}

📌 Actualizar un estudiante

PUT /api/estudiantes/{id}

Cuerpo JSON:

{
  "nombre": "María",
  "apellido": "González",
  "email": "maria.gonzalez@example.com",
  "fechaNacimiento": "2001-08-22",
  "numeroInscripcion": "S002"
}

📌 Eliminar un estudiante

DELETE /api/estudiantes/{id}



