# Git Kata: Branchement de Base

## Configuration

1. Exécutez `source setup.sh` (ou `.\setup.ps1` dans PowerShell)

## La tâche

Vous vivez à nouveau dans votre propre branche, cette fois-ci nous jonglerons un peu avec les branches, pour montrer à quel point les branches sont légères dans git.
Astuce : `git checkout` vous permettra de passer d'une branche à une autre.

1. Utilisez `git branch` pour voir les deux branches qui sont pertinentes pour cet exercice.
2. Sur quelle branche êtes-vous ?
3. Utilisez `git branch mybranch` pour créer une nouvelle branche appelée _mybranch_.
4. Utilisez à nouveau `git branch` pour voir la nouvelle branche créée.
5. Utilisez `git checkout mybranch` pour basculer sur votre nouvelle branche.
6. Comment la sortie de `git status` change-t-elle lorsque vous passez de la branche _master_ à la nouvelle branche que vous avez créée ?
7. Comment l'espace de travail change-t-il lorsque vous passez d'une branche à l'autre ?
8. Assurez-vous d'être sur votre branche _mybranch_ avant de continuer.
9. Créez un fichier appelé `file1.txt` avec votre nom comme contenu.
10. `add` le fichier et `commit` avec cette modification.
11. Utilisez `git log --oneline --graph` pour voir votre branche pointant vers le nouveau commit.
12. Revenez à la branche appelée _master_.
13. Utilisez `git log --oneline --graph` et remarquez comment le commit que vous avez fait sur la branche _mybranch_ est manquant sur la branche _master_.
14. Créez un nouveau fichier appelé `file2.txt` et commitez ce fichier.
15. Utilisez `git log --oneline --graph --all` pour voir votre branche pointant vers le nouveau commit, et que les deux branches ont maintenant des commits différents.
16. Basculez sur votre branche _mybranch_.
17. Qu'est-il arrivé à votre répertoire de travail ? Pouvez-vous voir votre `file2.txt` ?
18. Utilisez `git diff mybranch master` pour voir la différence entre les deux branches.

## Commandes utiles

- `git checkout`
- `git checkout -b`
- `git log --oneline --graph`
- `git branch`
- `git diff`
