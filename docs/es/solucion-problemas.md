---
title: Solución de Problemas
description: Solución de problemas comunes en RecWERTY: grabación, audio, efectos, errores de librería y logs.
---

# Solución de problemas

## La grabación no inicia

1. Verificá que FFmpeg esté instalado: `ffmpeg -version` en terminal.
2. Comprobá que el micrófono esté seleccionado correctamente.
3. Si usás zona personalizada, asegurate de haber dibujado el rectángulo.

## El audio no se graba

1. Verificá que el micrófono no esté silenciado en Windows.
2. Comprobá la selección de dispositivo en el panel de inicio.
3. Revisá los logs en `Documentos\RecWERTY\temp\recwerty.log`.

## El video renderizado no tiene efectos

1. Verificá que los efectos estén activados en la configuración.
2. Si usás preset **Raw/limpio**, los efectos están desactivados por diseño.

## Error de librería `libwertyaudio`

- Si ejecutás desde código fuente, asegurate de tener las dependencias de audio.
- Si usás el ejecutable compilado, verificá que el archivo `.pyd` esté presente.

## El ejecutable compilado no funciona

1. Revisá los logs bootstrap en la carpeta `temp/` junto al `.exe`.
2. Asegurate de que FFmpeg esté accesible desde el `PATH` del sistema.
3. Verificá que los assets estén generados (`generate_assets.py`).

## Dónde encontrar los logs

- **Modo desarrollo**: `Documentos\RecWERTY\temp\recwerty.log`
- **Modo ejecutable**: `temp\recwerty.log` (junto al .exe) y `Documentos\RecWERTY\temp\recwerty.log`
- **Bootstrap**: `temp\recwerty-bootstrap.log`

## Reportar problemas

Si encontrás un bug o tenés una sugerencia, abrí un issue en el repositorio del proyecto con:

- Versión de RecWERTY.
- Pasos para reproducir el problema.
- Logs relevantes.
- Captura de pantalla si aplica.
