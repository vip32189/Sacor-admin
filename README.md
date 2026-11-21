# Sancor-admin

Panel administrativo público sin pantalla de código local. Permite publicar `data/config.json` en `vip32189/Sancor` con un fine-grained PAT limitado a ese repositorio y permiso Contents: Read and write.

## Seguridad

Cualquiera puede abrir el panel. El token no se guarda en el repositorio ni en localStorage, pero debe entrar manualmente cada vez que se publique. Usa un token breve, revócalo si se expone y no lo compartas.
