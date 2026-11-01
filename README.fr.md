[English](README.md) | [日本語](README.ja.md) | [한국어](README.ko.md) | [Bahasa Indonesia](README.id.md) | **Français** | [繁體中文](README.zh-TW.md)

# Audio Device Restorer for OBS

Quand OBS change un périphérique audio sans prévenir, restaurez votre configuration en **un clic ou avec un raccourci** : volume, sourdine et, en option, les filtres avec les réglages des plugins VST. Le plugin VST lui-même n'est pas sauvegardé.

> Testé sur : OBS Studio 32.2.2, Windows 11. Langues : EN / JP / KR / ID / FR / TW
> Version 1.6.0 ・ Auteur : ChromeBread feat. BlackDream ・ Licence : GPL-2.0

## Préréglages et éléments à restaurer

<img src="docs/images/fr/audio_settings.png" alt="Réglages des préréglages et des éléments à restaurer" width="400">

Choisissez ce qui est restauré : périphérique, volume, sourdine, balance, monitoring, décalage de synchro et filtres. Tout est coché par défaut sauf les filtres.

## Utilisation
1. Dans OBS, ouvrez **Outils → Scripts → +** et sélectionnez `audio_device_restorer.lua`.
2. Réglez vos sources. Choisissez des **périphériques précis** plutôt que « Par défaut ».
3. Saisissez un nom de préréglage et cliquez sur **Enregistrer l'état actuel**.
4. Quand un périphérique change, cliquez sur **Restaurer le préréglage**.

Le raccourci se règle dans **Paramètres → Raccourcis**.

## Autres fonctions
- Plusieurs préréglages, vérification des différences
- Restauration automatique lors d'un changement et au démarrage d'OBS (désactivée par défaut)
- 9 emplacements de sauvegarde automatique pour annuler une erreur
- Enregistrement protégé des coupures de courant, avec reprise automatique depuis `.bak`
- Export / import des réglages de filtres, transfert des préréglages vers un autre PC

## Voir dans un dock OBS

<img src="docs/images/fr/audio_dock.png" alt="Dock avec une ligne rouge pour un périphérique différent" width="440">

Le dock affiche le contenu des préréglages et signale en rouge les périphériques différents.

Cochez **Mode débogage** pour afficher les chemins de fichiers, dont l'URL du dock. Une confirmation évite de les montrer en direct, et le mode se désactive à chaque ouverture des réglages.

## Désinstallation
Retirez le script dans **Outils → Scripts** (sélection, puis **−**), fermez OBS, puis lancez `Safe_Uninstaller.bat`. Il indique le rôle de chaque fichier, vous laisse choisir quoi supprimer, sauvegarde vos réglages, explique le passage à un autre PC et envoie le tout à la Corbeille.

Le détail complet est disponible en [English](README.md).

Ce script tiers n'est pas officiel. Il n'est ni affilié au projet OBS ni approuvé par celui-ci.
