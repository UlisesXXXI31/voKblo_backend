🚀 voKblo DE - API Backend (v1.0)
Este es el motor de servidor de voKblo DE, una plataforma EdTech diseñada para la gamificación del aprendizaje de alemán nivel B1. La API gestiona la autenticación segura, el progreso de los alumnos y un sistema dinámico de ranking.

🛠️ Stack Tecnológico
Runtime: Node.js

Framework: Express.js

Base de Datos: MongoDB Atlas (Mongoose ODM)

Seguridad: BcryptJS (Hashing de contraseñas)

Despliegue: Vercel

🏗️ Arquitectura y Funcionalidades Clave
El backend está estructurado para soportar una experiencia de aprendizaje interactiva:


Autenticación Robusta: Registro y login de usuarios con encriptación de seguridad.


Sistema de Gamificación (XP): Gestión dinámica de puntos y ranking (Leaderboard) integrada en tiempo real.


Panel Docente: Endpoints específicos para que el profesor supervise el historial detallado y el progreso de los alumnos.


Persistencia de Datos: Conexión escalable con MongoDB Atlas para el almacenamiento de estadísticas y perfiles de usuario.

📋 Endpoints Principales
Autenticación
POST /users/register - Registro de nuevos alumnos/profesores.

POST /auth/login - Acceso seguro y recuperación de perfil.

Progreso y Ranking
POST /progress - Actualización de XP y registro de lecciones completadas.

GET /leaderboard - Obtención de los 10 mejores estudiantes para el ranking.

Gestión Educativa (Profesor)
GET /users - Listado completo de alumnos matriculados.

GET /progress/:userId - Historial académico detallado de un estudiante específico.

⚙️ Instalación y Configuración
Clona el repositorio.

Instala dependencias: npm install.

Configura el archivo .env con tu MONGODB_URI.

Ejecuta en local: npm start.
