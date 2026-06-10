---
title: Installing RecWERTY
description: Installation from source code with git and uv, or from a compiled executable on Windows.
---

# Installation

## From source code

```bash
# 1. Clone the repository
git clone <repo-url>
cd recwerty

# 2. Install dependencies
uv sync

# 3. Optional: install build dependencies (to compile executable)
uv sync --extra build

# 4. Generate assets (sounds, images)
uv run python generate_assets.py

# 5. Run
uv run python main.py
```

## Compiled executable (Windows)

If you have the compiled executable (`.exe`), simply run it. User data is stored at:

- **Configuration**: `%APPDATA%\RecWERTY\`
- **Recordings**: `Documents\RecWERTY\recordings\`
- **Brand presets**: `Documents\RecWERTY\brands\`
- **Temporary files**: `Documents\RecWERTY\temp\`

!!! tip "Audio dependencies"
    If running from source, make sure you have the required audio dependencies. For the compiled executable, verify that the corresponding `.pyd` file is present.
