# Sancor-admin

Panel estático en español para administrar presentación, servicios, precios, duración, imágenes por URL, horarios semanales y excepciones de fecha.

## Activar GitHub Pages

Este repositorio contiene el panel en la rama `main`, raíz del repositorio. En **Settings → Pages → Build and deployment**, elige **Deploy from a branch**, selecciona `main` y `/(root)`, y pulsa **Save**.

URL: `https://vip32189.github.io/Sacor-admin/` una vez que termine el despliegue.

## Uso del panel y publicación directa

1. Abre el panel y configura el código local (barrera visual únicamente).
2. Edita presentación, servicios y disponibilidad. Se guardan en el almacenamiento local de ese navegador.
3. Para publicar automáticamente, crea en GitHub un **fine-grained personal access token** con expiración, acceso únicamente al repositorio `vip32189/Sancor` y permiso de repositorio **Contents: Read and write**. No uses un token clásico ni habilites permisos adicionales.
4. Pega el token en el campo del panel y elige **Publicar configuración**. El navegador lo usa para leer el SHA actual y actualizar `data/config.json` mediante GitHub Contents API. El campo se limpia al finalizar; el token no se guarda en `localStorage` ni en el repositorio.
5. También puedes descargar `config.json` y actualizarlo manualmente. Las imágenes deben tener una URL pública HTTPS.

## Seguridad importante

Este método requiere escribir el token en el navegador; durante el uso, el token está disponible para la página y se transmite a `api.github.com`. Úsalo solo desde el dominio oficial de GitHub Pages y un dispositivo confiable. No lo pegues en chats ni lo guardes en los archivos del repositorio. Configura expiración corta y revoca el token inmediatamente si sospechas que se expuso. Todo token con acceso de escritura puede modificar contenido del repositorio dentro de su alcance.

El código local no autentica al administrador de manera segura. GitHub Pages no ofrece backend, base de datos, sincronización entre navegadores ni bloqueo de horarios. Las reservas se envían por WhatsApp y requieren confirmación manual; pueden ocurrir solicitudes simultáneas para la misma hora.
