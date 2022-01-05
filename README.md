<h1 align="center">NOTFLIX Baguette 🇫🇷🥖 - Powershell</h1>
<p align="center">Utiliser la version française de notflix pour voir les prochains films avec Kev Adams 🍷</p>

##
<p align="center">
<img src="./preview.gif" alt="Video Preview" width="500px">
</p>

> [la vidéo de bugswriter's](https://youtu.be/RFJCL9C46Mc)

### Mais Jamy comment ça marche ?

C’est simple, il s’agit un script shell. Il extrait les infos de **oxtorrent** et trouve le lien *magnet*.
Ensuite, il utilise [webtorrent](https://webtorrent.io/) pour diffuser la vidéo à partir du lien.
Pour l'extraction, le script utilise des utilitaires gnu simples (sed, awk, paste, cut) mais aussi xmllint.

## Les trucs nécessaires

* [webtorrent-cli](https://webtorrent.io) - Un client de streaming peer-to-peer.
* [BurntToast](https://github.com/Windos/BurntToast) - Pour afficher les notifications.
* Avoir deja lancer internet explorer...
* [Du pain](https://youtu.be/biRzNHnvoC0?t=22)...

## L'Installation

### Avec Start-BitsTransfer
Télécharger **notflix-fr** avec Start-BitsTransfer et ajouter le dans votre **$env:PATH** et autoriser l'exécution des script.

```sh
Start-BitsTransfer "https://raw.githubusercontent.com/lunar-d/notflix-FR/win32/notflix" -Destination "~\notflix-fr.ps1"
Set-ExecutionPolicy RemoteSigned -scope CurrentUser
```
- Pour désinstaller, supprimez simplement `notflix-fr.ps1`.

## La licence
Ce projet est sous la licence publique générale GNU [GPL-3.0](http://www.gnu.org/licenses/gpl-3.0.txt).