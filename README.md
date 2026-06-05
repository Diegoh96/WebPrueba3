# WebPrueba3
# Veterinaria Patitas Felices

## Descripción

Aplicación web desarrollada con Node.js, Express y MySQL para gestionar productos de una veterinaria.

Permite:

- Registrar productos.
- Listar productos.
- Consultar productos por ID.
- Validar datos.
- Conectarse a una base de datos MySQL.
- Proteger endpoints mediante API Key.

---

## Tecnologías Utilizadas

### Frontend

- HTML5
- CSS3
- JavaScript

### Backend

- Node.js
- Express

### Base de Datos

- MySQL Workbench
- mysql2

---

## Estructura del Proyecto

```text
proyecto-productos

backend
│
├── src
│   ├── config
│   ├── controllers
│   ├── data
│   ├── middlewares
│   ├── routes
│   ├── services
│   └── server.js

frontend
│
├── index.html
├── style.css
└── app.js
```

---

## Instalación

### Instalar dependencias

```bash
npm install
```

### Ejecutar servidor

```bash
npm run dev
```

---

## Base de Datos

```sql
CREATE DATABASE veterinaria;

USE veterinaria;

CREATE TABLE productos(
id INT AUTO_INCREMENT PRIMARY KEY,
nombre VARCHAR(100),
precio DECIMAL(10,2),
stock INT
);
```

---

## Endpoints

### Obtener productos

```http
GET /api/productos
```

### Obtener producto por ID

```http
GET /api/productos/:id
```

### Crear producto

```http
POST /api/productos
```

Headers:

```http
x-api-key: 123456
```

Body:

```json
{
  "nombre":"Vacuna",
  "precio":15000,
  "stock":20
}
```

---

## Seguridad

Se implementó una API Key para proteger los endpoints de escritura.

La API Key evita que usuarios no autorizados registren información en el sistema.

---

## HTTPS

HTTPS protege la información enviada entre cliente y servidor mediante cifrado SSL/TLS.

Beneficios:

- Protege credenciales.
- Protege datos personales.
- Evita ataques Man In The Middle.
- Garantiza integridad de la información.

---

## Evidencias

- Captura de estructura del proyecto.
- Captura de MySQL Workbench.
- Captura de Postman.
- Captura del servidor ejecutándose.
- Captura del formulario funcionando.
- Captura de GitHub y commits.
