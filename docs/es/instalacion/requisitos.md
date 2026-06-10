---
title: Requisitos del Sistema
description: Requisitos mínimos y recomendados para ejecutar RecWERTY v3.2 en Windows.
---

# Requisitos del sistema

| Componente | Requisito |
|---|---|
| **Sistema operativo** | Windows 10 u 11 (64 bits) |
| **Python** | 3.13 o superior |
| **RAM** | 8 GB mínimo (16 GB recomendado) |
| **GPU** | NVIDIA (NVENC), Intel (QuickSync) o AMD (AMF) para codificación acelerada |
| **Disco** | 500 MB para la aplicación, más espacio para grabaciones |
| **FFmpeg** | Instalado y accesible en `PATH` |

## Dependencias de software

- **Python 3.13+**: [Descargar Python](https://www.python.org/downloads/)
- **uv**: Gestor de paquetes

    ```powershell
    powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
    ```

- **FFmpeg**: [Descargar FFmpeg](https://ffmpeg.org/download.html) y agregarlo al `PATH`

!!! warning "FFmpeg es obligatorio"
    Sin FFmpeg instalado y accesible desde `PATH`, RecWERTY no puede procesar ni codificar videos. Verificá la instalación con `ffmpeg -version` en una terminal.
