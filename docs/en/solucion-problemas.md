---
title: Troubleshooting
description: Common issues in RecWERTY — recording, audio, effects, library errors, and logs.
---

# Troubleshooting

## Recording won't start

1. Verify that FFmpeg is installed: `ffmpeg -version` in terminal.
2. Check that the microphone is selected correctly.
3. If using custom region, make sure you drew the rectangle.

## Audio not recording

1. Verify that the microphone is not muted in Windows.
2. Check the device selection on the home panel.
3. Review logs at `Documents\RecWERTY\temp\recwerty.log`.

## Rendered video has no effects

1. Verify that effects are enabled in settings.
2. If using the **Raw/clean** preset, effects are disabled by design.

## `libwertyaudio` library error

- If running from source, make sure you have the audio dependencies.
- If using the compiled executable, verify that the `.pyd` file is present.

## Compiled executable doesn't work

1. Check bootstrap logs in the `temp/` folder next to the `.exe`.
2. Make sure FFmpeg is accessible from the system `PATH`.
3. Verify that assets are generated (`generate_assets.py`).

## Where to find logs

- **Development mode**: `Documents\RecWERTY\temp\recwerty.log`
- **Executable mode**: `temp\recwerty.log` (next to the .exe) and `Documents\RecWERTY\temp\recwerty.log`
- **Bootstrap**: `temp\recwerty-bootstrap.log`

## Reporting issues

If you find a bug or have a suggestion, open an issue in the project repository with:

- RecWERTY version.
- Steps to reproduce the problem.
- Relevant logs.
- Screenshot if applicable.
