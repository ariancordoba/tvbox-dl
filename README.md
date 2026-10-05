# tvbox-dl

Descargas del launcher de los TV box. **Solo archivos publicados, sin código.**

- `config.json`: configuración que reciben los boxes. Va **firmada** (ECDSA P-256): los boxes descartan
  cualquier cambio que no esté firmado con la clave privada, que no está en este repo.
- Release `launcher-latest`: el APK del launcher (firmado con la clave de la app; Android rechaza
  cualquier otro como actualización).

Los boxes lo leen a través de `https://api.neonplayok.com/tvbox/config` y `/tvbox/launcher.apk`.
