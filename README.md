<h1 align="center">NOTFLIX Baguette 🇫🇷🥖</h1>
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

## Les truc nécessaires

* [webtorrent-cli](https://webtorrent.io) - Un client de streaming peer-to-peer.
* [libxml](http://www.xmlsoft.org) - Bibliothèque utilisée pour analyser les fichiers XML.
* [dmenu](https://webtorrent.io/) - Un menu dynamique pour X.
* [Du pain](https://youtu.be/biRzNHnvoC0?t=22).

## L'Installation

### Avec cURL
Télécharger **notflix-fr** avec cURL dans votre **$PATH** et autoriser l'exécution.

```sh
$ sudo curl -sL "https://raw.githubusercontent.com/lunar-d/notflixFR/master/notflix" -o /usr/local/bin/notflix-fr
$ sudo chmod +x /usr/local/bin/notflix-fr
```
- Pour mettre à jour, il suffit de refaire `curl`, plus besoin de `chmod`.
- Pour désinstaller, supprimez simplement `notflix-fr` de votre **$PATH** (`sudo rm -f /usr/local/bin/notflix-fr.`)

## La licence
Ce projet est sous la licence publique générale GNU [GPL-3.0](http://www.gnu.org/licenses/gpl-3.0.txt).

