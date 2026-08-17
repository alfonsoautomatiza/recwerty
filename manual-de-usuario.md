---
created: 2026-08-13
tags:
  - contexto/proyecto/manual
---
# Manual de Usuario — RecWERTY v3.2.3

> **RecWERTY**: Grabación de pantalla profesional con efectos de movimiento y mejora de audio.
> Versión 3.2.3 | Windows | Microsoft Store ID: `9NLD6GX4L1R1`

---

## Índice

1. [¿Qué es RecWERTY?](#qué-es-recwerty)
2. [Requisitos del sistema](#requisitos-del-sistema)
3. [Instalación](#instalación)
4. [Primeros pasos](#primeros-pasos)
5. [Interfaz principal](#interfaz-principal)
6. [Modos de captura](#modos-de-captura)
7. [Grabación](#grabación)
8. [Efectos y movimiento](#efectos-y-movimiento)
9. [Audio](#audio)
10. [Personalización de marca (Branding)](#personalización-de-marca-branding)
11. [Ajustes y configuración](#ajustes-y-configuración)
12. [Procesamiento y renderizado](#procesamiento-y-renderizado)
13. [Cola de renderizado](#cola-de-renderizado)
14. [Importar y procesar videos existentes](#importar-y-procesar-videos-existentes)
15. [Exportación para redes sociales](#exportación-para-redes-sociales)
16. [Exportación a GIF](#exportación-a-gif)
17. [Atajos de teclado](#atajos-de-teclado)
18. [Licencia y actualizaciones](#licencia-y-actualizaciones)
19. [Presets y respaldos](#presets-y-respaldos)
20. [Solución de problemas](#solución-de-problemas)

---

## ¿Qué es RecWERTY?

RecWERTY es una herramienta de grabación de pantalla profesional diseñada para crear **demos de software** y **videos tutoriales** de forma rápida, sin necesidad de edición. Grabás tu pantalla y obtenés un video pulido con efectos visuales, mejora de audio y personalización de marca al instante.

### Capacidades principales

- **Grabación de pantalla**: Pantalla completa, ventanas específicas o regiones personalizadas.
- **Efectos visuales en tiempo real**: Ripples de clic, estela del cursor, partículas y transiciones.
- **Sonidos de teclado**: Sonidos polifónicos que siguen tu tipeo, con variación por tipo de tecla.
- **Mejora de audio**: Filtros de estudio para voz, reducción de ruido, compresión y ecualización.
- **Personalización de marca**: Intros animadas con logo, colores corporativos y tipografía.
- **Exportación optimizada**: Presets para YouTube, TikTok, Instagram, Twitter/X y más.
- **Exportación a GIF**: GIFs optimizados de alta calidad.
- **Cola de renderizado**: Procesá múltiples trabajos en paralelo.

---

## Requisitos del sistema

| Componente | Requisito |
|---|---|
| **Sistema operativo** | Windows 10 u 11 (64 bits) |
| **RAM** | 8 GB mínimo (16 GB recomendado) |
| **GPU** | NVIDIA (NVENC), Intel (QuickSync) o AMD (AMF) para codificación acelerada |
| **Disco** | 500 MB para la aplicación, más espacio para grabaciones |

### Canal de instalación

- **Microsoft Store ID**: `9NLD6GX4L1R1`
- **Vínculo de Microsoft Store**: disponible después de publicar RecWERTY en Microsoft Store.
- **Deep link de Windows**: disponible después de publicar RecWERTY en Microsoft Store.
- **Actualizaciones**: llegan por Microsoft Store / Partner Center. RecWERTY no usa un actualizador propio dentro de la aplicación.

---

## Instalación

### Microsoft Store

Instalá RecWERTY desde Microsoft Store cuando la publicación esté disponible. El vínculo público se agregará al manual después de publicar la app.

### Ejecutable compilado (Windows)

Si tenés el ejecutable compilado (`.exe`), simplemente ejecutalo. Los datos de usuario se guardan en:

- **Configuración**: `%APPDATA%\RecWERTY\`
- **Grabaciones**: `Documentos\RecWERTY\recordings\`
- **Presets de marca**: `Documentos\RecWERTY\brands\`
- **Temporales**: `Documentos\RecWERTY\temp\`

---

## Primeros pasos

1. Abrí RecWERTY. Se abre en pantalla completa con una interfaz oscura moderna.
2. En el panel lateral izquierdo, seleccioná **Inicio**.
3. Elegí tu **modo de captura**: Pantalla completa, Ventana o Zona personalizada.
4. Configurá las opciones de audio, marca y efectos desde los paneles laterales.
5. Hacé clic en **LANZAR GRABACIÓN**.

---

## Interfaz principal

La interfaz de RecWERTY tiene un diseño oscuro tipo "Nothing" con acentos en rojo (#D71921).

### Panel de navegación (sidebar izquierdo)

| Icono | Sección | Descripción |
|---|---|---|
| 🏠 | **Inicio** | Panel principal de grabación |
| 🎨 | **Marca** | Personalización de marca y presets |
| ⚙️ | **Ajustes** | Configuración general de la app |
| 📋 | **Cola** | Cola de renderizado |
| ℹ️ | **Acerca de** | Información de la aplicación |

### Barra de estado superior

Muestra:
- Modo de captura activo
- Estado de la grabación
- Atajos disponibles (Alt+R para detener, Alt+Z para zoom)

---

## Modos de captura

RecWERTY ofrece tres modos de captura:

### Pantalla completa
Capturá todo el monitor. Si tenés múltiples monitores, seleccionás cuál usar desde el desplegable.

### Ventana
Seleccioná una ventana específica para grabar. RecWERTY lista automáticamente las ventanas activas visibles. Ideal para grabar una aplicación sin distracciones.

### Zona personalizada
Dibujá un rectángulo en pantalla para capturar solo esa región. Aparece una guía visual para que ajustes el área exacta. Presioná **ESC** para cancelar.

---

## Grabación

### Antes de grabar

Configurá estas opciones en el panel de inicio:

- **Microfono**: Seleccioná el dispositivo de entrada o desactivarlo.
- **Sonido del sistema**: Activá o desactivá la captura de audio del sistema.
- **Intro personalizada**: Activá para incluir una intro animada con tu marca.
- **Efectos de movimiento**: Clics, estela del cursor, partículas.

### Durante la grabación

- Aparece un **ícono en la bandeja del sistema** indicando que estás grabando.
- **Alt+R**: Detener grabación.
- **Alt+Z**: Activar/desactivar zoom manual.
- El timer overlay muestra el tiempo transcurrido.

### Después de grabar

Aparece el diálogo **Post-Recording**:

1. **Vista previa**: Reproducí el video grabado.
2. **Opciones de fondo**: Elegí entre:
   - **Auto**: Fondo generado automáticamente desde el color del video.
   - **Predefinido (HD)**: Fondos premium predefinidos.
   - **Ninguno**: Sin fondo adicional.
3. **Conservar o eliminar**: Elegí si quedarte con la grabación o descartarla.

Si elegís conservarla, se abre el procesador de video donde podés ajustar efectos antes del render final.

---

## Efectos y movimiento

RecWERTY incluye un sistema completo de efectos visuales que se aplican automáticamente a tu grabación.

### Efectos de clic

| Efecto | Descripción |
|---|---|
| **Ripple** | Onda expansiva estilo Material Design en la posición del clic |
| **Pulse** | Destello circular que pulsan en el punto del clic |
| **Sparkle** | Partículas brillantes que estallan en el clic |
| **Ninguno** | Sin efecto visual |

### Estela del cursor

- **Comet trail**: Estela brillante que sigue al cursor con degradado de color.
- Configurable: largo de la estela, radio del brillo, intensidad.
- Colores extraídos de tu marca si está configurada.

### Destello del cursor

Resalta el cursor con un brillo adicional cuando hace clic.

### Efectos de partículas

Sistema de partículas para agregar dinamismo a la escena durante la grabación.

### Transiciones

| Transición | Descripción |
|---|---|
| **Ninguna** | Corte directo |
| **Crossfade** | Disolvencia clásica |
| **Slide left** | Deslizamiento hacia la izquierda |
| **Zoom in** | Acercamiento |
| **Wipe left** | Barrido |
| **Circle reveal** | Revelado circular |
| **Glitch** | Efecto de falla digital |

### Sonidos de teclado polifónicos

Sistema de sonidos que reproduce variaciones según:

- **Tipo de tecla**: Letras, espacio, enter, backspace, modificadores, números, símbolos, flechas.
- **Velocidad de tipeo**: Ajusta el volumen según qué tan rápido escribís.
- **Múltiples variaciones**: Evita el sonido robótico con samples aleatorios.

---

## Audio

### Mejora de voz (Studio)

RecWERTY aplica filtros de audio profesionales usando FFmpeg:

- **Normalización**: Ajusta el volumen a un nivel uniforme (-24 LUFS).
- **Filtro pasa-bajos**: Elimina frecuencias agudas molestas (9 kHz).
- **Filtro pasa-altos**: Elimina ruidos de baja frecuencia (80 Hz, pisadas, rumbos).
- **Reducción de ruido**: Limpia el ruido de fondo.
- **Compresión**: Ecualiza los picos de volumen.
- **Ecualización de voz**: Potencia las frecuencias vocales.

### Configuración de audio

En el panel de inicio:

- **Micrófono**: Seleccionar dispositivo de entrada.
- **Sonido del sistema**: Grabar o no el audio del sistema.
- **Mejora de voz**: Activá/desactivá el procesamiento de estudio.
- **Normalizar audio**: Uniformizar el volumen general.
- **Sonidos de clic**: Activá/desactivá sonidos de mouse.
- **Sonidos de teclado**: Activá/desactivá sonidos de tecleo.

---

## Personalización de marca (Branding)

El sistema de marca te permite crear intros animadas profesionales con los colores de tu empresa.

### Panel de Marca

1. **Logo**: Subí el logo de tu empresa (PNG, JPG). RecWERTY extrae automáticamente los colores predominantes.
2. **Nombre de la empresa**: El nombre que aparecerá en la intro.
3. **Colores**: Primario, secundario y acento. Se detectan automáticamente del logo o los podés ajustar manualmente.
4. **Tipografía**: Seleccioná la fuente para los textos.
5. **Template de intro**: Elegí entre:
   - **Logo Reveal**: Intro cinematográfica de 3s con brillo.
   - **Minimal Fade**: Fundido elegante de 1.5s.

### Presets de marca

Podés crear múltiples presets para diferentes clientes o proyectos:

- **Guardar preset**: Guardá la configuración actual como un preset.
- **Cargar preset**: Cambiá entre presets guardados.
- **Importar preset (`.recbrand`)**: Compartí presets como archivos ZIP con marca.
- **Exportar preset**: Exportá un preset como archivo `.recbrand`.

La aplicación auto-aplica el preset configurado al iniciar.

### Diálogo de Branding

Accesible desde el panel de Marca. Incluye:

- Preview de la intro animada.
- Ajuste manual de colores con selectores.
- Subida de logo con arrastrar y soltar.
- Configuración de "The End" con logo, email y teléfono.

---

## Ajustes y configuración

### Ajustes de exportación

| Opción | Valores | Descripción |
|---|---|---|
| **Preset** | Demo rápida, Alta calidad, Raw/limpio, Social | Configuración predefinida de exportación |
| **Calidad** | 720p, 1080p, 1440p, source | Resolución de salida |
| **Directorio de salida** | Personalizable | Dónde se guardan los videos |
| **Intención** | demo, quality, raw, social | Ajusta los parámetros según el propósito |
| **CRF** | 12–30 (menor = mejor calidad) | Control de calidad del video |
| **Preset FFmpeg** | ultrafast, fast, medium, slow | Velocidad de compresión vs calidad |

### Presets de exportación

| Preset | Calidad | CRF | FFmpeg | Efectos |
|---|---|---|---|---|
| **Demo rápida** | 1080p | 20 | medium | Predeterminados |
| **Alta calidad** | 1440p | 17 | slow | Highlight cursor + partículas |
| **Raw/limpio** | source | 18 | medium | Raw mode, sin mejora de voz |
| **Social** | 1080p | 21 | fast | Crossfade en transiciones |

### Ajustes generales

- **Licencia**: Activación de licencia PRO.
- **Versiones nuevas**: Publicadas por el instalador oficial o Microsoft Store / Partner Center.
- **Idioma**: Español, English, Français.

---

## Procesamiento y renderizado

Cuando terminás una grabación, RecWERTY procesa el video aplicando:

1. **Efectos Studio**: Clics, cursor, partículas, transiciones.
2. **Banda de sonido**: Mezcla de audio con mejora de voz.
3. **Intro**: Generación y superposición de la intro animada.
4. **Render final**: Codificación con FFmpeg (acelerada por GPU si está disponible).

El procesamiento muestra una barra de progreso con el estado actual. Podés seguir grabando mientras se procesa gracias al sistema de cola.

---

## Cola de renderizado

La cola de renderizado permite procesar múltiples videos en paralelo.

### Características

- **Máximo 2 trabajos simultáneos**: Para no saturar el sistema.
- **Cola FIFO**: Los trabajos se procesan en orden.
- **Pausar/Reanudar**: Podés pausar la cola sin cancelar los trabajos en curso.
- **Cancelar**: Cancelación limpia de trabajos individuales.
- **Notificaciones**: Signals de progreso por trabajo.

### Acceso

Desde el panel lateral: **Cola** (ícono de lista). Allí ves:

- Nombre del trabajo
- Barra de progreso individual
- Estado: pending, rendering, completed, failed
- Botón para cancelar/pausar

---

## Importar y procesar videos existentes

Podés importar videos ya grabados para aplicarles los efectos de RecWERTY.

### Import Video Dialog

1. Hacé clic en **IMPORT VIDEO & APPLY EFFECTS** desde la pantalla principal.
2. Seleccioná el archivo de video.
3. Opciones disponibles:
   - **Trim**: Recortá el inicio y final del video.
   - **Fondo**: Elegí fondo automático, predefinido o ninguno.
   - **Grabación de voz en off**: Grabá una narración sobre el video importado.

### Procesamiento

El video importado pasa por el mismo pipeline de efectos que una grabación nueva (efectos de clic, transiciones, intro, mejora de audio).

---

## Exportación para redes sociales

RecWERTY incluye presets optimizados para plataformas sociales.

### Presets disponibles

| Plataforma | Resolución | FPS | Bitrate | Máx. duración |
|---|---|---|---|---|
| **YouTube** | 1920×1080 | 60 | 12 Mbps | Sin límite |
| **TikTok** | 1080×1920 | 30 | 6 Mbps | 3 min |
| **Instagram Reel** | 1080×1920 | 30 | 6 Mbps | 90 seg |
| **Twitter/X** | 1280×720 | 30 | 5 Mbps | 2 min 20 seg |
| **LinkedIn** | 1280×720 | 30 | 5 Mbps | 10 min |
| **WhatsApp** | 720×1280 | 30 | 2 Mbps | 16 min |

### Cómo usar

1. Configurá la grabación con el preset **Social**.
2. O usá el preset manual desde ajustes de exportación.
3. Al procesar, seleccioná la plataforma destino.

---

## Exportación a GIF

Podés exportar segmentos de tus videos como GIFs animados optimizados.

### Presets de GIF

| Preset | Ancho máx. | FPS | Colores | Dithering |
|---|---|---|---|---|
| **Alta calidad** | 800px | 15 | 256 | Floyd-Steinberg |
| **Balanceado** | 600px | 10 | 128 | Bayer |
| **Rápido** | 400px | 8 | 64 | Ninguno |

### Uso

Seleccioná la opción de exportación GIF desde el diálogo post-grabación o desde la biblioteca de videos.

---

## Atajos de teclado

| Atajo | Acción |
|---|---|
| **Alt + R** | Detener grabación |
| **Alt + Z** | Activar/desactivar zoom manual |
| **ESC** | Cancelar selección de zona |
| **Ctrl + Shift + R** | Iniciar captura rápida (atajo global) |

Los atajos se muestran en la interfaz durante la grabación.

---

## Licencia y actualizaciones

### Estado de licencia

- **PRO**: Funcionalidad completa con mejora de voz, codificación GPU y todas las resoluciones.
- **UNLICENSED**: Modo limitado. Activá desde Ajustes > Licencia.

### Activación

1. Andá a **Ajustes** > **Licencia & actualizaciones**.
2. Ingresá tu clave de licencia.
3. Hacé clic en **Activar**.

### Actualizaciones

- Las versiones para usuarios finales se publican por Microsoft Store / Partner Center o como nueva versión del instalador oficial.
- RecWERTY no usa un actualizador propio dentro de la aplicación.
- La versión actual se muestra en la pantalla Acerca de.

### Archivos de licencia y configuración

- **Config**: `Documentos\RecWERTY\config.ini`
- **Licencia**: `Documentos\RecWERTY\licencia.lic`
- **Logs**: `Documentos\RecWERTY\temp\recwerty.log`

---

## Presets y respaldos

### Sistema de presets de marca

Los presets se guardan en `Documentos\RecWERTY\brands\` con esta estructura:

```
brands/
├── current.txt              # Preset activo
├── backups/                 # Respaldos automáticos
├── recents.json             # Últimos 5 presets usados
├── mi-cliente/              # Preset individual
│   ├── brand.json           # Configuración de marca
│   ├── assets/
│   │   ├── logo.png         # Logo del cliente
│   │   └── end_logo.png     # Logo de cierre
│   └── metadata.json        # Metadatos del preset
└── ...
```

### Respaldos automáticos

- RecWERTY crea un respaldo del preset actual al iniciar la aplicación.
- Se conservan los últimos **3 respaldos**.
- Los respaldos viejos se podan automáticamente.

### Formato `.recbrand`

Los presets se exportan/importan como archivos `.recbrand` (ZIP conteniendo `brand.json`, `metadata.json` y `assets/`).

### Política de conflictos al importar

| Política | Comportamiento |
|---|---|
| **rename** | Agrega sufijo `_N` al nombre (por defecto) |
| **overwrite** | Reemplaza el preset existente |
| **skip** | No importa si ya existe |

---

## Solución de problemas

### La grabación no inicia

1. Comprobá que elegiste un modo de captura.
2. Si usás zona personalizada, asegurate de haber dibujado el rectángulo.
3. Cerrá otras apps que puedan bloquear la captura de pantalla y probá otra vez.

### El audio no se graba

1. Verificá que el micrófono no esté silenciado en Windows.
2. Comprobá la selección de dispositivo en el panel de inicio.
3. Revisá los logs en `Documentos\RecWERTY\temp\recwerty.log`.

### El video renderizado no tiene efectos

1. Verificá que los efectos estén activados en la configuración.
2. Si usás preset **Raw/limpio**, los efectos están desactivados por diseño.

### Error de librería `libwertyaudio`

- Reiniciá RecWERTY y probá otra vez.
- Si el error continúa, enviá un reporte con la versión de RecWERTY y los pasos para reproducirlo.

### El ejecutable compilado no funciona

1. Confirmá que usás Windows 10 u 11 de 64 bits.
2. Abrí RecWERTY desde el menú Inicio.
3. Si Windows muestra SmartScreen, revisá que el archivo venga del canal oficial antes de continuar.

### Dónde encontrar los logs

- **Logs de la app**: `Documentos\RecWERTY\temp\recwerty.log`

### Reportar problemas

Si encontrás un bug o tenés una sugerencia, abrí un issue en el repositorio del proyecto con:
- Versión de RecWERTY.
- Pasos para reproducir el problema.
- Logs relevantes.
- Captura de pantalla si aplica.

---

## Notas técnicas

### Directorios de datos de usuario

| Propósito | Ruta |
|---|---|
| Grabaciones | `Documentos\RecWERTY\recordings\` |
| Presets de marca | `Documentos\RecWERTY\brands\` |
| Archivos temporales | `Documentos\RecWERTY\temp\` |
| Recuperación | `Documentos\RecWERTY\recovery\` |
| Fuentes | `Documentos\RecWERTY\fonts\` |
| Herramientas | `Documentos\RecWERTY\tools\` |
| Configuración | `%APPDATA%\RecWERTY\settings.json` |

### Formatos de salida

- **Video**: MP4 (H.264/H.265 con aceleración GPU)
- **Audio**: AAC 48kHz estéreo
- **GIF**: GIF animado optimizado
- **Snapshot**: PNG

### Codificación acelerada por GPU

RecWERTY detecta y usa automáticamente:
- **NVIDIA NVENC** (tarjetas NVIDIA)
- **Intel QuickSync** (gráficos integrados Intel)
- **AMD AMF** (tarjetas AMD)

---

*RecWERTY v3.2.3 | Documentación para usuarios finales*
