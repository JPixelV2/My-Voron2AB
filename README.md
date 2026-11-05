# Voron 2.2 Afterburner — copia de configuración

Impresora de JPixelV2. Backup reparado el 5 de noviembre de 2026.

La carpeta `voron-config/` contiene los archivos de `~/printer_data/config/`, con los enlaces de KAMP, Mainsail y timelapse convertidos en copias de su contenido para poder recuperarlos.

Se excluyen archivos de secretos y claves, temporales, archivos comprimidos y la carpeta OLD. `telegram.conf` se incluye sin credenciales; el token y el identificador del chat se guardan por separado en un archivo privado fuera de esta copia. Las credenciales se conservan por separado y no deben publicarse. El historial antiguo del repositorio puede contener credenciales previamente publicadas: deben revocarse.

El backup usa Klipper-Backup y una clave SSH de escritura limitada a este repositorio. El ejecutor comprueba el acceso y verifica que el commit local coincide con GitHub. No copia configuraciones desde GitHub hacia la impresora.

Para restaurar: conservar primero la configuración existente, descargar la revisión deseada de `voron-config/`, revisar compatibilidad con el hardware y las versiones instaladas, reponer los secretos por separado y copiar los archivos a `~/printer_data/config/`. Revisar los componentes de Moonraker y las extensiones de Klipper antes de reiniciar. Este repositorio no sustituye una imagen completa de la tarjeta SD.

Telegram: version estable v2.1.0, conexion directa con Moonraker en 127.0.0.1:7125. El token publicado anteriormente se revoco el 5 de noviembre de 2026. Para restaurar el bot, reponer su archivo privado de secretos o generar un token nuevo con BotFather; no publicar credenciales.
