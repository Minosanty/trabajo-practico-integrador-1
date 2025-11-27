
# Trabajo Práctico Integrador 1

API REST desarrollada con **Express.js** y **Sequelize** para la gestión de artículos, usuarios, etiquetas y autenticación.

## 📋 Requisitos Previos

- **Node.js** v16 o superior
- **npm**
- **MySQL** v8 o superior (o compatible)

## 🚀 Instalación

### 1. Clonar el repositorio

```bash
git clone https://github.com/Minosanty/trabajo-practico-integrador-1.git
cd trabajo-practico-integrador-1
```

### 2. Instalar dependencias

```bash
npm install
```

### 3. Configurar variables de entorno

Crea un archivo `.env` en la raíz del proyecto con las siguientes variables:

```env
PORT=3000
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=tu_contraseña
DB_NAME=nombre_base_datos
DB_PORT=3306
JWT_SECRET=tu_jwt_secret
```

> Nota: Ajusta los valores según tu entorno local o de despliegue.





## 📦 Dependencias Principales

- **express** - Framework web
- **sequelize** - ORM para MySQL
- **mysql2** - Driver de MySQL
- **jsonwebtoken** - Autenticación JWT
- **bcrypt** - Hashing de contraseñas
- **express-validator** - Validación de datos
- **cors** - Control de acceso entre dominios
- **dotenv** - Gestión de variables de entorno

## 🎯 Scripts Disponibles

```bash
# Ejecutar en modo desarrollo con auto-recarga
npm run dev

# Ejecutar en producción (si no hay script "start", usa node app.js)
node app.js
```

> En este proyecto `package.json` proporciona `dev` para desarrollo. Puedes añadir un script `start` si quieres usar `npm start`.

## 📂 Estructura del Proyecto

```
src/
├── config/          # Configuración de base de datos
├── controllers/     # Lógica de negocio
├── models/          # Modelos Sequelize
├── routes/          # Definición de rutas
├── middlewares/     # Middlewares personalizados
├── helpers/         # Funciones auxiliares (JWT, bcrypt)
└── validations/     # Validaciones de datos
```

## 🔑 Rutas Principales

- `/auth` - Autenticación (login, registro)
- `/users` - Gestión de usuarios
- `/articles` - Gestión de artículos
- `/tags` - Gestión de etiquetas
- `/article-tags` - Relación artículos-etiquetas

Revisa los archivos en `src/routes` para confirmar paths y métodos exactos.

## 👨‍💻 Autor

SANTIAGO MIÑO
