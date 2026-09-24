# Guía de Despliegue e Instalación del Sistema

## 1. Requisitos Previos del Servidor
Paara poner en marcha la aplicación e-commerce, se requiere disponer del siguiente entorno:
*  **Servidor Web:** Node.js v18.x o superior.
*  **Base de Datos:** PostgreSQL v15.0.
*  **Menoria RAN Mínima:** 2 GB RAM / 2 Cores CPU.
*  **Sistema Operativo:** Ubuntu Server 22.04 LTS (Recomendado).
  
## 2. Procedimiento  de Instalación Técnicacmente Despachado

### Paso 2.1: Oobtención del Código fuente 
El administrador del sistema debe clonar el repositorio remoto inicial desde la plataforma Github hacia  el servidoor de destino y navegar a la carpeta raíz del proyecto.

### Paso 2.2: Instalación de Dependencias del Proyecto
Se deben instalar los paquetes y denpnedecias requeridas mediante el gestor de paquetesden entorno Node.
js, ejecutando el descarga automáticamente descrita en el archivo de configuración.

### Paso 2.3: Cnfiguraci´´on de Variables de Entonrno
Crea un archivo llamado `.env` en la raíz del proyecto tomando como base el archivo `.evn.example`, definiendo los parámetros de conexión:
* Puerto de red del servicio (`PORT`)
* Dirrección de host de la base de datos (`DB_HOST`)
* Puerto de base de datos (`DB_PORT`)
* Usuario y clave de acceso a la base de daatos (`DB_USER`, `DB_PASS`)

### Paaso 2.4: Puesta en Marcha del Servicio
Iniciar el servicio wed en modo de desarrollo o producción verificando en la consola que los puertos de enlace estén abiertos y escuchando peticiones.