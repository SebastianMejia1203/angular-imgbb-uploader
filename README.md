# Angular ImgBB Uploader

Aplicación web para seleccionar una imagen, previsualizarla y subirla a ImgBB desde el navegador. Devuelve la URL de la imagen alojada y muestra notificaciones sobre el resultado de la operación.

## Funcionalidades

- Selección y vista previa de archivos locales.
- Entrada de una API key de ImgBB desde la interfaz.
- Carga mediante HTTP y formulario multipart.
- Visualización del enlace devuelto por ImgBB.
- Notificaciones de selección, validación, éxito y error.

## Tecnologías

Angular 17.1, TypeScript, RxJS, Bootstrap 5 y ngx-toastr.

## Inicio local

Necesitas Node.js y npm compatibles con Angular 17, además de una API key de ImgBB para realizar cargas.

```bash
npm ci
npm start
```

Abre `http://localhost:4200`, selecciona una imagen, introduce tu API key y ejecuta la carga. La imagen se envía al servicio externo ImgBB.

## Comandos

| Comando | Propósito |
| --- | --- |
| `npm start` | Servidor de desarrollo |
| `npm run build` | Compilación en `dist/` |
| `npm test` | Pruebas con Karma y Jasmine |

## Estructura

- `src/app/app.component.*`: interfaz, vista previa y flujo de carga.
- `src/app/services/api-upload.service.ts`: integración con la API de ImgBB.
- `src/app/app.config.ts`: configuración de la aplicación.
