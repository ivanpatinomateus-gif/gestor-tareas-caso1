# Requisitos del Proyecto - Gestor de Tareas en Equipo (Caso 1)

## Actores
- **Integrante del equipo / Usuario**: Persona encargada de gestionar, asignar y actualizar el estado de las tareas.

## Requisitos Funcionales (RF)
- **RF1**: El sistema debe permitir crear una tarea con título, descripción, responsable, estado y fecha límite.
- **RF2**: El sistema debe permitir listar todas las tareas registradas.
- **RF3**: El sistema debe permitir consultar una tarea específica por su ID.
- **RF4**: El sistema debe permitir editar o actualizar los datos de una tarea existente.
- **RF5**: El sistema debe permitir cambiar el estado de una tarea (pendiente, en progreso, hecha).
- **RF6**: El sistema debe permitir asignar una tarea a un integrante del equipo.
- **RF7**: El sistema debe permitir eliminar una tarea por su ID.
- **RF8**: El sistema debe permitir filtrar tareas por estado (`?estado=...`) o por responsable (`?responsable=...`).

## Requisitos No Funcionales (RNF)
- **RNF1**: La API debe responder exclusivamente en formato JSON.
- **RNF2**: Los campos `titulo` y `responsable` no pueden estar vacíos al crear una tarea.
- **RNF3**: Se deben utilizar códigos de estado HTTP estándar (200, 201, 204, 400, 404).
