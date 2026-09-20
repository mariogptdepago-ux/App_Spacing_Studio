# Sistema de Aplicaciones HTML Seguras

Repositorio listo para la instalación del sistema con **Google Apps Script + Google Sheets + Google Drive**.

## Roles

- **ADMINISTRADOR**: administra usuarios, carga/elimina aplicaciones, activa/desactiva, programa horarios y consulta informes.
- **DOCENTE**: activa/desactiva aplicaciones, programa horarios, abre prácticas y consulta informes.
- **ESTUDIANTE**: únicamente abre las prácticas para las que tiene permiso y genera/consulta sus propios informes.

## Aplicaciones iniciales

El proyecto incluye dos prácticas iniciales:

1. Razones relacionadas · AP4 · EJE1 · D1 · Grado 11.
2. Refuerzo acumulativo · AP4 · EJE1 · D1 · Grado 11.

En el primer arranque se copian automáticamente a una carpeta privada de Google Drive y quedan **DESACTIVADAS**. Después de iniciar sesión, el Administrador o Docente puede activarlas mediante interruptores.

## Qué subir a GitHub

Sube **todo el contenido de este repositorio**.

Se recomienda configurar el repositorio como **PRIVATE**, porque contiene los HTML fuente de las prácticas iniciales.

## Archivos de Apps Script

Dentro de `apps_script/` están todos los archivos necesarios:

- `Code.gs`
- `Index.html`
- `appsscript.json`
- `App_Numerico_AP4_EJE1_D1_Grado11.html`
- `App_RefuerzoAcumulativo_AP4_EJE1_D1_Grado11.html`

## Instalación inicial

GitHub se utiliza como repositorio del código. La ejecución se realiza en Google Apps Script.

1. Cree una hoja de cálculo de Google Sheets.
2. Abra **Extensiones → Apps Script**.
3. Copie `Code.gs`.
4. Cree `Index.html` y copie su contenido.
5. Cree los dos archivos HTML de aplicaciones con exactamente estos nombres:
   - `App_Numerico_AP4_EJE1_D1_Grado11`
   - `App_RefuerzoAcumulativo_AP4_EJE1_D1_Grado11`
6. Active la visualización de `appsscript.json` en Configuración del proyecto y reemplace su contenido.
7. Despliegue como **Aplicación web**:
   - Ejecutar como: **yo**.
   - Acceso: **cualquier persona con el enlace**.
8. Abra la URL generada.
9. El primer acceso mostrará el asistente para crear la cuenta **ADMINISTRADOR**.
10. Inicie sesión. Las dos prácticas iniciales aparecerán en el menú como **desactivadas**.
11. Active las que desee.
12. Desde **Usuarios**, cree cuentas DOCENTE y ESTUDIANTE y asigne permisos a los estudiantes.

## Uso cotidiano

Después de la instalación, los responsables no necesitan usar GitHub.

- ADMINISTRADOR: gestiona todo desde el panel.
- DOCENTE: activa/desactiva y programa con clics.
- ESTUDIANTE: selecciona una práctica autorizada y la abre.

Los nuevos HTML pueden cargarse desde **+ Cargar nuevo HTML** por un ADMINISTRADOR. Nacen desactivados.

## Seguridad incluida

- Autenticación con usuario y contraseña.
- Roles verificados en el backend.
- Permisos por aplicación.
- Activación/desactivación central.
- Programación de fecha/hora.
- Sesiones temporales.
- HTML guardados en carpeta privada de Drive.
- Bloqueo de ejecución local (`file://`) en las copias servidas.
- Bloqueo disuasorio de clic derecho y atajos comunes.
- Aviso de confidencialidad, propiedad intelectual y uso con IA.
- Registro de auditoría e informes.

### Límite técnico

Ninguna aplicación web puede garantizar que una persona autorizada no haga una captura de pantalla, transcriba contenido o modifique una copia del código que haya logrado obtener. El aviso para IA es una medida declarativa y disuasoria, no una barrera universal. La protección principal consiste en mantener las aplicaciones en Drive privado, verificar permisos en servidor y servirlas solo a sesiones autorizadas.
