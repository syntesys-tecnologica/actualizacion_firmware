# Informe técnico — Actualización de firmware y estandarización de NVR

Aplicación web de una sola página (`index.html`) para capturar el registro fotográfico de la configuración de los NVR en las tiendas Dollarcity y generar el informe en PDF.

## Funciones
- 97 casillas de captura en orden (firmware, System, Network, Video/Audio, Image, Event, Storage, Orden de servicio).
- Motion Detection y Record Schedule por cámara (Cámara 1 a 24).
- Foto con la cámara o desde la galería, repetir o saltar casilla.
- Guardar y cargar avance (`.json`) para continuar después.
- Descarga de todas las fotos en ZIP.
- Informe PDF con portada, carta de presentación y fotos (6 por hoja en Motion Detection y Record Schedule, 2 por hoja en el resto).

## Publicar en GitHub Pages
1. Crea un repositorio nuevo en GitHub.
2. Sube `index.html`, `README.md` y `.nojekyll` a la raíz del repositorio.
3. Ve a **Settings → Pages**.
4. En **Build and deployment** elige **Deploy from a branch**, rama `main` y carpeta `/ (root)`. Guarda.
5. En uno o dos minutos la app estará en `https://TU-USUARIO.github.io/NOMBRE-DEL-REPOSITORIO/`.

## Notas
- Requiere internet al abrirla: carga jsPDF y JSZip desde cdnjs.
- Las fotos no se suben a ningún servidor; todo se procesa en el navegador del dispositivo.
