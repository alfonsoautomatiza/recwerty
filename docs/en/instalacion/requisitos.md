---
title: System Requirements
description: Minimum and recommended requirements to run RecWERTY v3.2 on Windows.
---

# System requirements

| Component | Requirement |
|---|---|
| **Operating system** | Windows 10 or 11 (64-bit) |
| **Python** | 3.13 or higher |
| **RAM** | 8 GB minimum (16 GB recommended) |
| **GPU** | NVIDIA (NVENC), Intel (QuickSync), or AMD (AMF) for hardware encoding |
| **Disk** | 500 MB for the application, plus space for recordings |
| **FFmpeg** | Installed and accessible in `PATH` |

## Software dependencies

- **Python 3.13+**: [Download Python](https://www.python.org/downloads/)
- **uv**: Package manager

    ```powershell
    powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
    ```

- **FFmpeg**: [Download FFmpeg](https://ffmpeg.org/download.html) and add it to `PATH`

!!! warning "FFmpeg is required"
    Without FFmpeg installed and accessible from `PATH`, RecWERTY cannot process or encode videos. Verify the installation with `ffmpeg -version` in a terminal.
