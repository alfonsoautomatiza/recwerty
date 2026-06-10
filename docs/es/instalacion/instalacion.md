---
title: Instalación de RecWERTY
description: Instalación desde código fuente con git y uv, o desde ejecutable compilado en Windows.
---

# Instalación

## Desde código fuente

```bash
# 1. Clonar el repositorio
git clone <repo-url>
cd recwerty

# 2. Instalar dependencias
uv sync

# 3. Opcional: instalar dependencias de build (para compilar ejecutable)
uv sync --extra build

# 4. Generar assets (sonidos, imágenes)
uv run python generate_assets.py

# 5. Ejecutar
uv run python main.py
```

## Ejecutable compilado (Windows)

Si tenés el ejecutable compilado (`.exe`), simplemente ejecutalo. Los datos de usuario se guardan en:

- **Configuración**: `%APPDATA%\RecWERTY\`
- **Grabaciones**: `Documentos\RecWERTY\recordings\`
- **Presets de marca**: `Documentos\RecWERTY\brands\`
- **Temporales**: `Documentos\RecWERTY\temp\`

!!! tip "Dependencias de audio"
    Si ejecutás desde código fuente, asegurate de tener las dependencias de audio necesarias. Para el ejecutable compilado, verificá que el archivo `.pyd` correspondiente esté presente.
