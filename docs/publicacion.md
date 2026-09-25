# Publicación de la web de Killary

## Repositorio y despliegue

El sitio comercial se mantiene en **Jorbnc/Killary_Web**. Para publicar, configurar en **Settings → Pages** la fuente **Deploy from a branch**, rama **main** y carpeta **/(root)**. Los cambios posteriores se publican al subir los commits a esa rama.

Desde este repositorio, revisar los archivos, crear un commit y ejecutar `git push origin main`. El remoto ya existe; no repetir `git remote add origin`. El error inicial `src refspec main does not match any` se debía a que todavía no había ningún commit.

El despliegue y el repositorio son estados distintos. Revisar Pages/Actions y abrir las páginas sin iniciar sesión para comprobar que están disponibles.

## Direcciones

| Página | URL |
|---|---|
| Inicio | `https://jorbnc.github.io/Killary_Web/` |
| Privacidad del sitio | `https://jorbnc.github.io/Killary_Web/privacidad.html` |
| Condiciones del sitio | `https://jorbnc.github.io/Killary_Web/condiciones.html` |
| Dominio del sitio | `jorbnc.github.io` |

Estas políticas describen exclusivamente esta web comercial. Su publicación no acredita que otras aplicaciones que traten datos mediante las API de Google tengan la información de privacidad que requieren. No presentar estas políticas como documentación de funciones que no describen.

## Verificación de propiedad

Si se necesita verificar propiedad en Google, entrar en Search Console con la cuenta correspondiente, añadir una propiedad de prefijo de URL y seguir el método HTML ofrecido. Publicar la etiqueta o archivo exacto entregado por Google y verificar después del despliegue; conservarlo posteriormente. No inventar códigos de verificación.

- [Publicar en GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site).
- [Verificar propiedad en Google](https://support.google.com/webmasters/answer/9008080).
- [Configurar Branding](https://console.cloud.google.com/auth/branding).
- [Requisitos de Branding](https://support.google.com/cloud/answer/15549049).

## Vista previa y archivo opcional

Abrir `index.html` en un navegador. `dist/killary-web-pages.zip`, si está presente, contiene los tres HTML, CSS y `.nojekyll`. Es una copia de distribución excluida de Git; el mantenimiento normal se hace en los archivos fuente.
