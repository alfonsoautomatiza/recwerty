---
title: Prérequis Système
description: Configuration minimale et recommandée pour exécuter RecWERTY v3.2 sur Windows.
---

# Prérequis système

| Composant | Configuration requise |
|---|---|
| **Système d'exploitation** | Windows 10 ou 11 (64 bits) |
| **Python** | 3.13 ou supérieur |
| **RAM** | 8 Go minimum (16 Go recommandé) |
| **GPU** | NVIDIA (NVENC), Intel (QuickSync) ou AMD (AMF) pour l'encodage accéléré |
| **Disque** | 500 Mo pour l'application, plus d'espace pour les enregistrements |
| **FFmpeg** | Installé et accessible dans `PATH` |

## Dépendances logicielles

- **Python 3.13+** : [Télécharger Python](https://www.python.org/downloads/)
- **uv** : Gestionnaire de paquets

    ```powershell
    powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
    ```

- **FFmpeg** : [Télécharger FFmpeg](https://ffmpeg.org/download.html) et l'ajouter au `PATH`

!!! warning "FFmpeg est obligatoire"
    Sans FFmpeg installé et accessible depuis `PATH`, RecWERTY ne peut pas traiter ni encoder les vidéos. Vérifiez l'installation avec `ffmpeg -version` dans un terminal.
