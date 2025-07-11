# Aplicación de Control de Dividendos Internacionales

## Descripción
Esta aplicación permite gestionar el cobro de dividendos de empresas de cualquier país y divisa, calculando automáticamente el cambio a euros y las retenciones fiscales en origen y destino.

## Estructura
- **backend/**: API en FastAPI (Python)
- **frontend/**: Interfaz en React (JavaScript)

## Ejecución local

1. **Clona el repositorio**
2. **Arranca los servicios con Docker Compose:**

```bash
docker-compose up --build
```

- El backend estará en http://localhost:8000
- El frontend en http://localhost:3000

## Despliegue en Coolify

1. Sube el proyecto a tu repositorio (GitHub, GitLab, etc.)
2. En Coolify, crea una nueva aplicación y selecciona este repositorio.
3. Coolify detectará el `docker-compose.yml` y levantará ambos servicios automáticamente.

## Notas
- La base de datos es SQLite y se almacena en la carpeta `backend/`.
- La aplicación está preparada para ser migrada a producción fácilmente. 