# Killary Backup

Sitio informativo de la herramienta privada de respaldos de Killary, con política de privacidad y condiciones de uso para su configuración OAuth de Google Drive.

## Archivos

- `index.html`: portada y descripción del funcionamiento.
- `privacidad.html`: tratamiento de datos y autorizaciones.
- `condiciones.html`: condiciones de uso privado.
- `styles.css`: diseño adaptable a escritorio y móvil.
- `.nojekyll`: publicación estática en GitHub Pages.
- `docs/publicacion.md`: despliegue, URLs de Branding y verificación de propiedad.

HTML y CSS sin dependencias, scripts de seguimiento, formularios ni compilación. Para una vista previa, abrir `index.html` en el navegador.

## Publicación

En este repositorio, configurar **Settings → Pages → Deploy from a branch → main → /(root)**. La URL prevista es `https://jorbnc.github.io/Killary_Web/`; confirmar el despliegue en Pages antes de usarla en Google Cloud.

Consultar las [instrucciones completas](docs/publicacion.md). El sitio es independiente del proyecto operativo de Killary y no contiene datos del negocio, presupuesto, respaldos ni credenciales.

## Mantenimiento

Revisar que privacidad y condiciones correspondan al funcionamiento real antes de publicar cambios. Mantener enlaces relativos entre las páginas. El contacto público es el perfil de GitHub `jorbnc`; no añadir correos u otros datos personales sin indicación de su titular.

`dist/` contiene, cuando se genera, una copia ZIP para carga manual; se excluye de Git para evitar duplicar los archivos fuente. La aplicación de respaldos y su autorización OAuth se configuran aparte: publicar el sitio no las activa.
