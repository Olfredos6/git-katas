# Git Kata: Nettoyage de base

## Configuration

1. Exécutez `source setup.sh` (ou `.\setup.ps1` dans PowerShell)

## La tâche

Vous travaillez sur un projet qui implique des fichiers générés. Disons que vous compilez des fichiers de code, ecrits en langage de programmation C, en fichiers objet. Avant de passer à une nouvelle branche, vous voulez partir sur une base propre.

1. Explorez le répertoire avec `ls -R`. Il y a beaucoup de choses. Fichiers de code, fichiers temporaires, fichiers objet,.. Nettoyons tout !
2. Juste pour être sûr, faites un essai à sec et exécutez la commande de nettoyage [git clean](https://git-scm.com/docs/git-clean/fr) avec l'option `-n`.
3. Oh non ! Il y a un fichier `.c` qui aurait été supprimé !
4. Ajoutez `src/mylib.c` à la zone de transit. Ne le validez pas.
5. Exécutez la commande de nettoyage avec l'option `-n`. Remarquez que mylib.c ne sera pas supprimé. Remarquez également que les fichiers dans le répertoire obj ne sont pas répertoriés.
6. Exécutez la commande de nettoyage avec l'option `-n -d`.
7. C'est bon ! Nettoyez le dépôt avec `-f -d`.

## Commandes utiles

- `git clean -n`
- `git add`
- `git clean -n -d`
- `git clean -f -d`
