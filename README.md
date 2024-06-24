FastApi - Videogames

Esta API proporciona endpoints para gestionar una base de datos de videojuegos, incluyendo operaciones CRUD y autenticación de usuarios.

## Características

- Autenticación de usuarios con JWT
- CRUD completo para videojuegos
- Soft delete para videojuegos
- Base de datos PostgreSQL
- Documentación automática con Swagger UI

## Requisitos

- Python 3.8+
- PostgreSQL
- pip

## Instalación

1. Clonar el repositorio.
2. Crear un entorno virtual e instalar las dependencias:
3. Configurar la base de datos:
- Crear una base de datos PostgreSQL
- Actualizar la URL de la base de datos en `app/database.py`

4. Ejecutar la aplicación: uvicorn app.main:app --reload

## Uso

Una vez que la aplicación esté en ejecución, puedes acceder a la documentación de la API en:

- Swagger UI: `http://localhost:8000/docs`

### Autenticación

Para usar los endpoints protegidos, primero debes obtener un token JWT:

1. POST `/oauth/token` con tus credenciales de usuario
2. Usar el token recibido en el header `Authorization: Bearer <token>` para las siguientes peticiones

### Endpoints principales

- GET `/videogames/`: Listar todos los videojuegos
- POST `/videogames/`: Crear un nuevo videojuego
- GET `/videogames/{id}`: Obtener un videojuego específico
- PUT `/videogames/{id}`: Actualizar un videojuego
- DELETE `/videogames/{id}`: Eliminar (soft delete) un videojuego

## Desarrollo

Para contribuir al proyecto:

1. Crea un fork del repositorio
2. Crea una nueva rama para tu feature: `git checkout -b feature/AmazingFeature`
3. Haz commit de tus cambios: `git commit -m 'Add some AmazingFeature'`
4. Push a la rama: `git push origin feature/AmazingFeature`
5. Abre un Pull Request

## Licencia

Distribuido bajo la licencia MIT. Ver `LICENSE` para más información.

## Contacto

Jelsy Manuel Diaz Jiménez - jelsymdiazj@gmail.com

Link del Proyecto: 
