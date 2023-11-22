# Git Kata: Fusion Mergesort

Dans cette kata, vous serez confronté à un conflit de fusion et devrez le résoudre en modifiant le fichier en conséquence.

Vous travaillerez avec les deux branches suivantes:

* Mergesort-Impl
* master

La tâche consiste à examiner le conflit de fusion et à le résoudre en modifiant le fichier en conséquence.

## Configuration

1. Exécutez `source setup.sh` (ou `.\setup.ps1` dans PowerShell)

## La tâche

1. Exécutez `git branch` pour voir les deux branches présentes.
2. Fusionnez `Mergesort-Impl` dans `master`.
3. Soit :
   1. Résolvez le conflit de fusion avec votre éditeur préféré et terminez la fusion (`git status` vous dira quoi faire), **ou**
   2. Utilisez `git mergetool --tool=emerge` (pour les fans d'Emacs) ou `git mergetool --tool=vimdiff` (pour les fans de Vim) et terminez la fusion (`git status` vous dira quoi faire).

## Commandes pertinentes

- `git branch`
- `git merge`
- `git status`
- `git mergetool --tool=emerge`
- `git mergetool --tool=vimdiff`
- `git add`
- `git commit`
