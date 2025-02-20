# Quality-Control

## RELEASE 13/02/2025 v3.0.1 (SERVER) & RELEASE 13/02/2025 v2.9.0 (VERIFICADOR AUTOMATICO)  
```
VERIFICADOR AUTOMATICO  
```
- **Desactivar de la crankcase antes de empezar la verificación**
  - [x] [MOD]: Se mejora el POU para la desactivación de la resistencia del carter del compresor en los equipos MB4C  
- **Temperatura exterior**
  - [x] [MOD]: Se modifica la temperatura mínima para empezar una verficación, el rango es de 9º - 27º  
- **Lógica comunicación server - verificador automático**
  - [x] [FIX]: Finalizar verificación, mantiene comunicación entre server y verificador hasta que crea informe y deja el equipo preparado para cliente.  
```
SERVER  
```
- **Lógica para mantener la comunicación entre servidor y verificador en la finalización de la verificación**
  - [x] [Fix]: Refactorizar función comunicación entre server y verificador automático.

## RELEASE 19/01/2025 v3.0.0 (SERVER) 

```
BACKEND
```

- **Pruebas de conexión y base de datos:**
  - [x] [ADD]: Implementadas pruebas de conexión a la base de datos de infolinea, comunicación y consultas.
- **Refactorización de componentes:**
  - [x] [MOD]: Eliminados componentes innecesarios y se han agregado los componentes necesarios para la monoblock.  
- **Conexión a la base de datos:**
  - [x] [MOD]: Mejorada la conexión a la base de datos, estableciendo la conexión solo cuando se necesita.
- **Refactorización de respuestas de la base de datos:**
  - [x] [REF]: Ahora la base de datos devuelve los nombres de los campos o columnas de las tablas, en vez de los ID's.  
- **Refactorización del controlador de equipos:**
  - [x] [MOD]: Refactorizada la lógica para obtener y establecer un equipo para su verificación.
- **Corrección del registros de trazabilidad del modelo del Power+:**
  - [x] [Fix]: Corregido el nombre del modelo Power+.
- **Rutas de almacenamiento de informes:**
  - [x] [MOD]: Modificada la ruta de almacenamiento de informes de verificación y archivos de configuración del verificador automático.
- **Eliminación de consultas a Axapta:**
  - [x] [MOD]: Eliminadas consultas a Axapta.
- **Query de modificación de campo:**
  - [x] [ADD]: Se ha agregado un query para modificar un campo en la tabla de la base de datos de infolinea para indicar si la verificación ha sido exitosa o no.
- **Cambio de rutas para la instalación:**
  - [x] [MOD]: Se han cambiado las rutas para la instalación del software y cfield del equipo.
- **Variables de entorno:**
  - [x] [FIX]: Se han agregado variables de entorno para valores sensibles (nombre de usuario, contraseñas, puerto TCP, etc.).
- **Corrección del establecimiento de valores:**
  - [x] [FIX]: Corregido el establecimiento de valores en el verificador automático, como número de bombas, ventiladores, etc.
- **Formateo del número de serie:**
  - [x] [MOD]: Mejorado el formateo del número de serie para el escaneo de código de barras (23 caracteres / 9 caracteres / 13 caracteres).
- **Control de versiones semántico:**
  - [x] [ADD]: Implementado el control de versiones semántico, con cambios en los números de versión para indicar cambios incompatibles, agregado de nueva funcionalidad y correcciones.  
      El primer número cambia, cuando hay cambios incompatibles con la ultima versión. [BrokenChanges]  
      El segundo número cambia cuando se agrega una nueva funcionalidad y es compatible con última versión.  
      El tercer número cambia cuando se realiza alguna corrección y no rompe compatibilidad.  
- **Integración del frontend al backend:**
  - [x] [MOD]: Integración frontend / backend.
  
```
FRONTEND
```
    
  - [x] [MOD]: Logo, se ubica en el footer, para hacer area de verificación más amplia.  
  - [x] [MOD]: Area de alarmas, mejorada la visualización.  
  - [x] [ADD]: Se añade variable "currentVerification", si la aplicación cae, el servidor guarada en variable si hay una verificación en curso.  
  - [x] [ADD]: Nueva pantalla donde si existe una veerificaciión en curso, muestra dos botones (Continuar con verificación en curso ó Nueva verificación)  
  - [x] [Add]: Dos metodos que controlan la continuación de una verificación en curso o el inicio de una nueva verificación 

## RELEASE 11/12/2024 v2.8.3 (SERVER)  
```
SERVER
```
- [x] [ADD]: Nuevos códigos de articulos añadidos para equipos sin marca (7887123, 7887124, 7887125, 7887126)  
- [x] [ADD]: [DB_APP.json]  / CLIENT: [/verification/Equipo.vue, IconBlanc.vue]  
- [x] [ADD]: Imagen vectorizada, para  new svg for blanc brand. 

## RELEASE 9/10/2024  v2.8.2 (SERVER)

Primera maquina verificada con la nueva release: N/S 241000404  
  
- [x] [ADD]: Nuevos códigos de articulo para ventiladores (71182)  
- [x] [FIX]: Configuración de equipo, Abortar verificación y finalización de la verificación. 
- [x] [FIX]: Trazabilidad, siempres que comunique con el equipo después realiza la trazabilidad de nuevo. (Por sustitución de componente)  

---
