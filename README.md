# API REST - Gestión de Usuarios

Este proyecto muestra una implementación básica de una API RESTful utilizando **Node.js** y **Express**, con estructura modular y buenas prácticas de organización. Es útil como ejemplo introductorio para estudiantes o desarrolladores que desean comprender cómo desarrollar APIs REST.

## 🚀 Tecnologías utilizadas

- Node.js
- Express.js
- dotenv
- cors

## 📁 Estructura del proyecto

```
apirest-users/
├── controllers/
│   └── usuarios.js
├── models/
│   └── server.js
├── public/
│   └── 404.html (opcional)
├── routes/
│   └── usuarios.js
├── .env
├── app.js
└── package.json
```

## 🧩 Instalación y ejecución

1. Clona el repositorio:
```bash
git clone https://github.com/sdominguez/apirest-users.git
cd apirest-users
```

2. Instala las dependencias:
```bash
npm install
```

3. Crea un archivo `.env` en la raíz del proyecto con el siguiente contenido:
```
PORT=8081
```

4. Inicia el servidor:
```bash
node app.js
```

La API estará disponible en: `http://localhost:8081/api/usuarios`

La API estará disponible en: `http://localhost:8081/api/usuarios`

## 📌 Endpoints disponibles

| Método  | Endpoint                | Descripción                                                                 |
|---------|-------------------------|-----------------------------------------------------------------------------|
| GET     | /api/usuarios           | Retorna un mensaje de prueba con parámetros de consulta (`req.query`)      |
| POST    | /api/usuarios           | Envía nombre y edad como JSON en el cuerpo (`req.body`)                    |
| PUT     | /api/usuarios/:id       | Recibe un parámetro de segmento `id` y lo devuelve                         |
| PATCH   | /api/usuarios           | Retorna mensaje de prueba para PATCH                                       |
| DELETE  | /api/usuarios           | Retorna mensaje de prueba para DELETE                                      |

## 🔍 Ejemplos de uso

### GET con parámetros de consulta
```
GET /api/usuarios?q=test&nombre=Juan&apikey=1234&page=2&limit=10
```

Respuesta esperada:
```json
{
  "msg": " api GET desde controlador",
  "q": "test",
  "nombre": "Juan",
  "apikey": "1234",
  "page": "2",
  "limit": "10"
}
```

### POST con cuerpo JSON
```
POST /api/usuarios
Content-Type: application/json

{
  "nombre": "María",
  "edad": 25
}
```

Respuesta:
```json
{
  "msg": " api POST desde controlador",
  "nombre": "María",
  "edad": 25
}
```
