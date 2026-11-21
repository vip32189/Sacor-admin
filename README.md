# Sancor-admin

Panel estático en español para administrar presentación, servicios, precios, duración, imágenes por URL, horarios semanales y excepciones de fecha.

## Activar GitHub Pages

Este repositorio estaba vacío, por eso GitHub no ofrecía `main` como rama de publicación. Ahora que contiene estos archivos en la raíz y en la rama `main`, ve a **Settings → Pages → Build and deployment**, elige **Deploy from a branch**, selecciona `main` y `/(root)`, y pulsa **Save**.

La URL prevista es `https://vip32189.github.io/Sacor-admin/` una vez que termine el despliegue.

## Uso

1. Abre el panel desde la URL de GitHub Pages y crea un código local de al menos 12 caracteres.
2. Edita presentación, servicios y disponibilidad. La información se guarda en el almacenamiento local de ese navegador.
3. Descarga `config.json` desde el panel.
4. Reemplaza `data/config.json` en `vip32189/Sancor` por el archivo descargado y publica el cambio.

Las imágenes deben tener una URL pública HTTPS; no se cargan archivos de imagen desde el panel.

## Limitaciones de seguridad y operación

GitHub Pages no proporciona autenticación ni base de datos. El código local, cuyo hash se guarda en `localStorage`, es solo una barrera de interfaz; no protege el sitio de quienes inspeccionen o alteren el navegador. No guardes información sensible. No hay sincronización entre dispositivos, almacenamiento de reservas ni bloqueo de horarios. El cliente envía la solicitud por WhatsApp y el negocio debe confirmar disponibilidad. Los cambios se hacen públicos solo después de actualizar manualmente el archivo de configuración del repositorio Sancor.
