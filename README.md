# App_Spacing_Studio — GitHub Pages

Este repositorio público debe contener **solo la carcasa de acceso**.

Al abrir la URL de GitHub Pages, `index.html` carga dentro de la página la aplicación segura desplegada en Google Apps Script.

## Archivos

- `index.html`: entrada real de GitHub Pages.
- `config.js`: única configuración necesaria; contiene la URL pública `/exec` de Google Apps Script.
- `shell.js`: carga el sistema, bloquea ejecución local y aplica controles disuasorios.
- `styles.css`: apariencia de la carcasa.
- `404.html`: devuelve al inicio.
- `.nojekyll`: evita procesamiento innecesario de Jekyll.

## Configuración única

Después de desplegar el backend en Google Apps Script:

1. Copia la URL que termina en `/exec`.
2. Abre `config.js` en GitHub.
3. Sustituye:
   `PEGAR_AQUI_URL_APPS_SCRIPT`
   por la URL real.
4. Guarda el cambio.

Después de eso, la URL:

`https://TU-USUARIO.github.io/TU-REPOSITORIO/`

abre directamente el sistema de login/menú.

## IMPORTANTE

No subas a este repositorio público:

- HTML originales de las prácticas.
- `Code.gs`.
- `Index.html` del backend de Apps Script.
- contraseñas;
- tokens;
- hojas con usuarios;
- archivos con respuestas o bancos de preguntas.

Las prácticas deben permanecer en Google Drive privado y ser entregadas por el backend únicamente a usuarios autorizados.

## Roles del backend

- ADMINISTRADOR: usuarios, carga/eliminación de apps, activación, programación e informes.
- DOCENTE: activación/desactivación, programación, apertura de prácticas e informes.
- ESTUDIANTE: prácticas autorizadas e informes propios.

## Seguridad

La carcasa bloquea `file://`, clic derecho y atajos comunes de inspección. Estos controles son disuasorios. La seguridad principal corresponde al backend: autenticación, roles, permisos y almacenamiento privado de las aplicaciones.
