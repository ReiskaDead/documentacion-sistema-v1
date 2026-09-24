# Políticas y Protocolos de Seguridad del Sistema

## 1. Control de Accesos y Roles (RBAC)
El sistema aplica un esquema de Control de Acceso Basado en Roles para restringir operaciones sensibles:
* **Rol Cliente:** Acceso únicamente a lectura de productos y gestión de su propio carrito.
* **Rol Pasarela de Pagos:** Integración vía tokens cifrados para procesamiento de cobros.
* **Rol Administrador:** Acceso total a reportes, facturación y modificación de inventario.

## 2. Encriptación de Datos Sensibles
* Todas las contraseñas de los usuarios se almacenan encriptadas con el algoritmo **Bcrypt** (factor de costo 10).
* Todas las transmisiones web se ejecutan obligatoriamente sobre el protocolo **HTTPS (TLS 1.3)**.

## 3. Autenticación mediante Tokens
* La API emite firma digital mediante **JWT (JSON Web Tokens)** con tiempo de vida útil de 8 horas.
