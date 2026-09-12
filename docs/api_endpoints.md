# Especificación de Endpoints de la API

Esta sección decumentada los servicios wed (wed API) disponibles para la integración con otros sistemas.

## 1. Listado de Servicios web

| Método HTTP | Ruta / Endpoint | Descripción | Parámetros Exigidos |
| :-: | :--- | :--- | :--- |
| **GET** | `/api/v1/usuarios` | Obtiene el listado completado de usuarios registrados. | Ninguno |
| **POST** | `/api/v1/usuarios` | Registra un nuevo usuario en la base de datos . | `nombre`, `correo`,`rol` |
| **GET** | `/api/v1/reportes` | Genera y descarga el repote mensual en PDF. | `mes` (numéro) |

## 2. Códigos de Respiestas HTTP

> **Estándar de Errores:** Todos los Servicios responden utilizando códigos de estado HTTP estándar.

* **200 OK: ** La solicitud fue procesada exitosamente.
* **400 Bad Request:** Datos de entrada inválidos o faltantes.
* **404 Not Found:** El recurso solicitado no  existe en el servidor.
* **500 Internal Server Error:** Error interno en la lógica en Python o en la base de datos MySQL.
  
## 3. Ejemplo de Respuesta JSON
```JSON
{
    "status": 200,
    "message": "Usuarios resgistrado exitosamente",
    "data": {
        "id": 105,
        "nombre": "Carlos López",
        "rol": "Desarrollador"
    }
}
``` 

## 4. Navegación
- [Ver Manual de Usuario](manual_usuario.md)
- [Ver Arquitectura del Sistema] (arquitectura.md)
- [Volver al README Principal] (../README.md)