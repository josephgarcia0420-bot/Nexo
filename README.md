# NEXO 0.1.1

Finanzas personales con portada, registro e inicio de sesión, tema claro/oscuro, menú lateral, cuentas e ingresos/gastos. Paleta azul eléctrico, violeta y ámbar.

## Archivos

- `index.html`: portada y todas las pantallas.
- `styles.css`: diseño, temas y tipografía incorporada.
- `app.js`: acceso, movimientos, cuentas, cálculos y guardado.
- `icon.svg`, `icon-192.png`, `icon-512.png`, `apple-touch-icon.png`: identidad e icono de inicio.
- `manifest.webmanifest`: nombre, iconos y apertura como app desde la pantalla de inicio.
- `netlify.toml`: publicación y actualización de los archivos.

## Subir a GitHub

1. Descomprime el paquete.
2. Crea un repositorio NUEVO para Nexo en https://github.com/new . Mantén VYTRA en su propio repositorio.
3. En el repositorio, usa Add file → Upload files.
4. Sube todos los archivos de esta carpeta directamente a la raíz del repositorio. Debe verse `index.html` al abrir el repositorio. No subas únicamente el ZIP.
5. Guarda con Commit changes.

## Conectar con Netlify

1. Abre https://app.netlify.com/ .
2. Add new project → Import an existing project → GitHub.
3. Autoriza el acceso y selecciona el repositorio de Nexo.
4. Rama: `main` (o la rama que creaste). Base directory: vacío. Build command: vacío. Publish directory: `.` . No necesitas instalar dependencias ni ejecutar una compilación.
5. Pulsa Publish y abre la URL HTTPS asignada.
6. Las futuras actualizaciones en la rama conectada se publicarán desde GitHub en Netlify.

Referencia: https://docs.netlify.com/start/quickstarts/deploy-from-repository/

## iPhone

Abre la dirección HTTPS de Netlify en Safari. Usa Compartir → Añadir a pantalla de inicio. El icono y el nombre Nexo están incluidos. Esta versión requiere conexión para cargar; no incluye modo sin conexión.

## Datos y acceso

Este paquete contiene código de la app; no contiene tus movimientos ni tus contraseñas. Las cuentas y los movimientos son locales a cada navegador y dirección web. No hay acceso de servidor, respaldo remoto, sincronización o recuperación de contraseña. Crear un acceso en este prototipo no crea una cuenta en un servidor.

Al cambiar de un archivo de prueba a una dirección nueva de Netlify, los datos anteriores NO se trasladan automáticamente. Crea una cuenta de prueba en la nueva dirección. Mantén la misma dirección de Nexo para conservar los datos de ese navegador. Netlify aloja los archivos; no transforma el acceso local en autenticación real.

## Prueba local

En una computadora, desde esta carpeta: `python3 -m http.server 8000` . Abre `http://localhost:8000` . Para usarla desde otro dispositivo, publícala con HTTPS en Netlify.
