# Shell en C

Projet de création d'un shell, qui prend en charge les commandes externes et certaines commandes internes.

## Installation et utilisation 

Installer libreadline-dev "sudo apt install libreadline-dev"

Installer lncurse-dev "sudo apt-get install libncurses5-dev"

Pour compiler le projet, il suffit de lancer la commande 'make'.
Nous avons inclus les fichiers générés par bison et lex, mais pour les recompiler, on peut utiliser 'make yacclex'.

Il est possible comme prévu de créer un fichier ~/.mpshrc
Nous en avons fourni un exemple. Voici cependant quelques commentaires.
La variable INVITE définie le prompt de mpsh, il peut contenir trois variables :
- |u qui est remplacé par le nom d'utilisateur
- |w qui est remplacé par le chemin absolu vers le répertoire courant
- |W qui est remplacé par nom du répertoire courant
La variable CHEMIN peut-être redéfini, par défaut, il s'agit d'une copie de PATH.

La fonction complete prend en argument une commande ainsi qu'une expression régulière correspondant au fichier utilisable pour la complétion.

Le manuel des commandes internes se trouve dans manMPSH.man

## Contributeurs 

- Pierre Méjane
- Tristan François
- Omar Aldakar
