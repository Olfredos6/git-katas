# Git Kata: Rebaser une branche

## Configuration

1. Exécutez `source setup.sh` (ou `.\setup.ps1` dans PowerShell)

## La tâche

Vous vivez à nouveau dans votre propre branche, cette fois-ci nous jonglerons un peu avec les branches, pour montrer à quel point les branches sont légères dans git.

Cet exercice utilise la commande Git rebase. Vous pouvez en savoir plus à ce sujet [ici](https://git-scm.com/book/fr/v2/Les-branches-avec-Git-Rebaser-Rebasing).

1. Quelles branches existent ?
2. Regardez le journal pour la branche `master`.
3. Basculez sur la branche `uppercase`.
4. Comment le journal se compare-t-il au journal de la branche `master` ?
5. Rebasez votre branche `uppercase` sur la branche `master` (`git rebase master`).
6. Que s'est-il passé ? Dessinez-le !
7. Passez maintenant à la branche `master`.
8. Fusionnez `uppercase` dans `master`.
9. À quoi ressemble le journal maintenant ?

## Commandes utiles

- `git switch <nom-de-branche>`
- `git rebase <nom-de-branche>`
- `git log --oneline --graph --all`
- `git merge <nom-de-branche>`
