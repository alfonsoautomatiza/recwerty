---
title: Dépannage
description: Problèmes courants dans RecWERTY — enregistrement, audio, effets, erreurs de bibliothèque et logs.
---

# Dépannage

## L'enregistrement ne démarre pas

1. Vérifiez que FFmpeg est installé : `ffmpeg -version` dans un terminal.
2. Vérifiez que le microphone est correctement sélectionné.
3. Si vous utilisez une zone personnalisée, assurez-vous d'avoir dessiné le rectangle.

## L'audio ne s'enregistre pas

1. Vérifiez que le microphone n'est pas en sourdine dans Windows.
2. Vérifiez la sélection du périphérique sur le panneau d'accueil.
3. Consultez les logs dans `Documents\RecWERTY\temp\recwerty.log`.

## La vidéo rendue n'a pas d'effets

1. Vérifiez que les effets sont activés dans les paramètres.
2. Si vous utilisez le preset **Brut/propre**, les effets sont désactivés par conception.

## Erreur de bibliothèque `libwertyaudio`

- Si vous exécutez depuis le code source, assurez-vous d'avoir les dépendances audio.
- Si vous utilisez l'exécutable compilé, vérifiez que le fichier `.pyd` est présent.

## L'exécutable compilé ne fonctionne pas

1. Consultez les logs bootstrap dans le dossier `temp/` à côté du `.exe`.
2. Assurez-vous que FFmpeg est accessible depuis le `PATH` système.
3. Vérifiez que les assets sont générés (`generate_assets.py`).

## Où trouver les logs

- **Mode développement** : `Documents\RecWERTY\temp\recwerty.log`
- **Mode exécutable** : `temp\recwerty.log` (à côté du .exe) et `Documents\RecWERTY\temp\recwerty.log`
- **Bootstrap** : `temp\recwerty-bootstrap.log`

## Signaler un problème

Si vous trouvez un bug ou avez une suggestion, ouvrez un issue dans le dépôt du projet avec :

- Version de RecWERTY.
- Étapes pour reproduire le problème.
- Logs pertinents.
- Capture d'écran si applicable.
