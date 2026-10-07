# Diseño del Sistema - Gestor de Tareas

## 1. Modelo de Datos (Entidad Tarea)
- `id` (Número, autogenerado)
- `titulo` (Texto, obligatorio)
- `descripcion` (Texto, opcional)
- `responsable` (Texto, obligatorio)
- `estado` (Texto: "pendiente" | "en progreso" | "hecha", valor por defecto: "pendiente")
- `fechaLimite` (Texto/Fecha, opcional)

## 2. Rutas de la API (`/tareas`)

| Método | Ruta | Descripción |
| :--- | :--- | :--- |
| `GET` | `/tareas` | Lista todas las tareas (permite filtros `?estado=` y `?responsable=`) |
| `GET` | `/tareas/:id` | Obtiene los detalles de una tarea específica |
| `POST` | `/tareas` | Crea una nueva tarea |
| `PUT` | `/tareas/:id` | Edita o actualiza el estado/responsable de una tarea |
| `DELETE` | `/tareas/:id` | Elimina una tarea por ID |
