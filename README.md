# API REST Check Usuario TADS

## Descripción

Este proyecto consiste en una **API REST para la gestión y validación de usuarios**, desarrollada como parte de la práctica académica de la materia **Tecnologías y Aplicaciones de Desarrollo de Software (TADS)**.

La API permite realizar operaciones como:

* Registrar usuarios
* Validar acceso al sistema
* Consultar usuarios registrados
* Consultar tipos de usuario

Las pruebas de funcionamiento fueron realizadas utilizando **Postman**.

---

## Tecnologías utilizadas

* .NET Web API
* C#
* SQL Server
* Visual Studio
* Postman
* Git y GitHub

---

## Estructura del proyecto

apiRESTCheckUsuarioTADS

│

├── Controllers

├── Models

├── Data / Database

├── apiRESTBdUsuarioTADS.sln

└── README.md

---

## Endpoints de la API

### 1. Insertar Usuario

**Endpoint**

POST
/tads/usuario/spinsusuario

**Descripción**

Permite registrar un nuevo usuario en la base de datos.

**Ejemplo JSON**

```json
{
 "nombre": "Juan",
 "apPaterno": "Perez",
 "apMaterno": "Lopez",
 "correo": "juan@email.com",
 "password": "123456",
 "tipoUsuario": 1
}
```

---

### 2. Validar Acceso

**Endpoint**

POST
/tads/usuario/spvalidaracceso

**Descripción**

Permite validar las credenciales de acceso de un usuario.

**Ejemplo JSON**

```json
{
 "correo": "juan@email.com",
 "password": "123456"
}
```

---

### 3. Reporte de Usuarios

**Endpoint**

GET
/tads/usuario/vwrptusuario

**Descripción**

Obtiene la lista de usuarios registrados.

---

### 4. Reporte de Usuarios con Filtro

**Endpoint**

GET
/tads/usuario/vwrptusuario?nombre=&apPaterno=&apMaterno=

**Descripción**

Permite buscar usuarios aplicando filtros por:

* Nombre
* Apellido Paterno
* Apellido Materno

---

### 5. Tipos de Usuario

**Endpoint**

GET
/tads/usuario/vwtipousuario

**Descripción**

Obtiene los diferentes tipos de usuario disponibles en el sistema.

---



## Autor

Proyecto desarrollado por:

**Arely Tellez Salas**

Estudiante de Ingeniería en Tecnologías de la Información y Comunicaciones (ITIC)



Este proyecto fue desarrollado con fines académicos para demostrar la implementación de una **API REST utilizando buenas prácticas de desarrollo y control de versiones con GitHub**.
