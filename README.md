# Sancor-admin

Panel administrativo estático. Permite publicar `data/config.json` en `vip32189/Sancor` con un fine-grained PAT limitado a ese repositorio y permiso Contents: Read and write.

## Configuración

1. Activa GitHub Pages con `main /(root)`.
2. Abre el panel y crea el código local.
3. Crea un token fine-grained con acceso solo a `vip32189/Sancor`, permiso **Contents: Read and write**, expiración corta.
4. Pega el token al publicar. No se guarda.

## Riesgos

El código local no autentica realmente. El token solo debe usarse desde un dispositivo confiable y debe revocarse si se expone. El navegador exige que GitHub Pages use HTTPS. La reserva sigue siendo estática y debe confirmarse por WhatsApp.
