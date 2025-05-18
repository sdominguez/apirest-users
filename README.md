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

## 📌 Endpoints disponibles

| Método | Endpoint            | Descripción                         |
|--------|---------------------|-------------------------------------|
| GET    | /api/usuarios       | Obtener mensaje de prueba (GET)     |

> Puedes ampliar la funcionalidad agregando métodos POST, PUT, PATCH y DELETE en el controlador y las rutas.
