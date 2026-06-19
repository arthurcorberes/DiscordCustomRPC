# Discord Custom RPC

Affiche une Rich Presence Discord personnalisée, directement depuis le system tray.

## Prérequis

Avant d'installer DCRPC, il faut créer une application sur le **Discord Developer Portal** :

1. Rends-toi sur [discord.com/developers/applications](https://discord.com/developers/applications)
2. Clique sur **New Application** et donne-lui un nom : c'est ce nom qui apparaîtra sur ton profil Discord ("Playing **MonApp**")
3. Dans l'onglet **Rich Presence → Art Assets**, tu peux uploader des images qui serviront de `Large Image` et `Small Image`
4. Copie ton **Application ID** depuis la page General Information : tu en auras besoin dans DCRPC

## Installation

1. Télécharge `DCRPC.exe` depuis la page [Releases](../../releases)
2. Place-le où tu veux sur ton PC
3. Lance-le : il apparaît directement dans le **system tray** (barre des tâches en bas à droite)

## Configuration

1. Clic droit sur l'icône dans le tray → **Edit Presence**
2. Remplis les champs (certains sont facultatifs) :
   - **Client ID** — l'Application ID copié depuis le Developer Portal
   - **Details** — première ligne de ta présence (ex: `Customise son profil`)
   - **State** — deuxième ligne (ex: `à l'aide de DCRPC :P`)
   - **Large / Small Image Key** — nom exact de l'image uploadée sur le Developer Portal
   - **Button Label / URL** — un bouton cliquable affiché sur ta présence (visible uniquement par les autres)
3. Clique sur **Save** — la présence se met à jour immédiatement

## Démarrage automatique

Clic droit sur l'icône → **Launch at startup** pour activer ou désactiver le lancement au démarrage de Windows.

> **Note :** si le démarrage automatique est activé, DCRPC peut mettre **quelques minutes** à apparaître après le démarrage de la machine. Windows ne le considère pas comme une application prioritaire au boot, ce qui est tout à fait normal.

## Notes

- Le **bouton** de ta présence n'est pas visible pour toi sur Discord, c'est une limitation de Discord. Tes amis le voient parfaitement.
- Si la présence ne s'affiche pas, assure-toi que **Discord est ouvert** avant ou pendant le lancement de DCRPC. L'application réessaie automatiquement toutes les 10 secondes.
- La configuration est sauvegardée dans `%AppData%\DCRPC\config.json` (accessible via clic droit → **Open Config Folder**)
