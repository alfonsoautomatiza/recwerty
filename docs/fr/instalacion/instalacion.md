---
title: Installation de RecWERTY
description: Installation depuis le code source avec git et uv, ou depuis l'exécutable compilé sur Windows.
---

# Installation

## Depuis le code source

```bash
# 1. Cloner le dépôt
git clone <repo-url>
cd recwerty

# 2. Installer les dépendances
uv sync

# 3. Optionnel : installer les dépendances de build (pour compiler l'exécutable)
uv sync --extra build

# 4. Générer les assets (sons, images)
uv run python generate_assets.py

# 5. Exécuter
uv run python main.py
```

## Exécutable compilé (Windows)

Si vous disposez de l'exécutable compilé (`.exe`), lancez-le simplement. Les données utilisateur sont stockées dans :

- **Configuration** : `%APPDATA%\RecWERTY\`
- **Enregistrements** : `Documents\RecWERTY\recordings\`
- **Presets de marque** : `Documents\RecWERTY\brands\`
- **Fichiers temporaires** : `Documents\RecWERTY\temp\`

!!! tip "Dépendances audio"
    Si vous exécutez depuis le code source, assurez-vous d'avoir les dépendances audio nécessaires. Pour l'exécutable compilé, vérifiez que le fichier `.pyd` correspondant est présent.
