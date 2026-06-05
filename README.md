# WebPrueba3

Profe sali de ingles llegue a la casa y me di cuenta de mi error del .jon disculpe profesor estaba trabajando con una maqueta que había realizado antes y no fue la mejor idea y lo hice denuevo y un un error que me hago responsable dentro del backend no cree la dependencia npm init -y .json como todo que le meten ia nervioso lo hice a lo últimos 20min y descaradamente profe lo cree mal solo erar mover la carpeta del src a la carpeta de backend :c asumo la responsabilidad pero le pido disculpa y se que es muy tarde profe disculpe .
Profe por acá actualice el repositorio pero en el aula no profe solo el word.

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


## Como funciona en la terminal
npm install

npm install express mysql2 cors

npm install nodemon --save-dev

entra a la carpeta backend:
cd backend
y luego:
npm run dev
