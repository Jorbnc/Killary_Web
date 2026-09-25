# Publicación en GitHub Pages

El repositorio independiente del sitio es **Jorbnc/Killary_Web**. El usuario lo creó y pidió trasladar aquí los archivos públicos y sincronizarlos con el remoto. La portada, privacidad, condiciones y estilos se encuentran en la raíz.

## Actualizar el repositorio

Desde este repositorio, revisar los cambios antes de preparar el commit. Agregar únicamente los archivos públicos pertinentes, crear un commit y ejecutar `git push origin main`. No volver a ejecutar `git remote add origin` si ese remoto ya existe; consultar su valor con `git remote -v`.

El error `src refspec main does not match any` observado durante la creación ocurrió porque la rama todavía no tenía ningún commit. El commit inicial debe existir antes del primer `git push -u origin main`.

## Activar Pages

1. Abrir [Jorbnc/Killary_Web](https://github.com/Jorbnc/Killary_Web) en GitHub.
2. Entrar en **Settings → Pages → Build and deployment**.
3. Elegir **Deploy from a branch**, rama **main**, carpeta **/(root)**, y guardar.
4. Esperar a que termine el despliegue y usar **Visit site**.
5. Abrir las tres páginas sin iniciar sesión y comprobar enlaces, lectura y disposición en móvil antes de registrarlas en Branding.

El repositorio sincronizado no garantiza que Pages esté activado. Consultar su estado en Settings → Pages y en Actions. Los archivos están preparados para publicarse como estáticos, sin instalar Node ni compilar.

Referencias: [crear un sitio Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site), [fuente de publicación](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site).

## URLs para Branding

Usar estas URLs cuando su despliegue esté confirmado. Respetar las mayúsculas de `Killary_Web`:

| Campo | Valor |
|---|---|
| Application home page | `https://jorbnc.github.io/Killary_Web/` |
| Application privacy policy link | `https://jorbnc.github.io/Killary_Web/privacidad.html` |
| Application terms of service link | `https://jorbnc.github.io/Killary_Web/condiciones.html` |
| Authorized domains | `jorbnc.github.io` |

En Branding, mantener **Killary Backup** como nombre y el correo real del usuario como soporte/contacto. El correo público del sitio no se ha indicado; las páginas identifican a `jorbnc`, enlazan su perfil y remiten al correo de asistencia de OAuth. Publicar el sitio no verifica automáticamente la marca ni la propiedad ante Google, y tampoco activa los respaldos.

Si Google pide comprobar la propiedad, usar la cuenta propietaria/editora del proyecto OAuth en **Google Search Console**. Añadir una propiedad de **prefijo de URL** con la dirección exacta del sitio y seguir el método HTML ofrecido. Añadir la etiqueta `google-site-verification` proporcionada por Google al `<head>` de `index.html`, o publicar el archivo de verificación en la ubicación exacta indicada. No inventar el token. Volver a desplegar antes de verificar y conservar después la prueba de propiedad. Si Google exige otra dirección o dominio, resolver ese requisito concreto antes de dar la marca por aprobada. [Verificación de propiedad](https://support.google.com/webmasters/answer/9008080), [requisitos de Branding](https://support.google.com/cloud/answer/15549049).

## Paquete manual y vista previa

Abrir `index.html` en un navegador para revisar el sitio local. Todos los recursos propios y enlaces internos son relativos.

La copia opcional `dist/killary-backup-pages.zip` contiene únicamente `index.html`, `privacidad.html`, `condiciones.html`, `styles.css` y `.nojekyll` en su raíz. Se excluye de Git porque duplica el sitio y puede quedar desactualizada. Si se utiliza para cargar archivos manualmente, extraerlo antes: subir el ZIP no despliega su contenido. El flujo normal de mantenimiento es actualizar los archivos fuente y hacer commit/push.
