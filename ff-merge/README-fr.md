# Git Kata: Fusion Avant-Rapide

## Configuration

1. Exécutez `source setup.sh` (ou `.\setup.ps1` dans PowerShell)

## La tâche

Vous vivez à nouveau dans votre propre branche, cette fois-ci nous ferons jongler un peu avec les branches, pour montrer à quel point les branches sont légères dans git.

1. Créez une branche (feature) appelée `feature/uppercase` (oui, `feature/uppercase` est un nom de branche parfaitement légal et une convention courante).
2. Basculez sur cette branche.
3. Quelle est la sortie de `git status` ?
4. Modifiez le fichier `greeting.txt` pour contenir une salutation en majuscules.
5. Ajoutez le fichier `greeting.txt` à la zone de transit et commit.
6. Quelle est la sortie de `git branch` ?
7. Quelle est la sortie de `git log --oneline --graph --all` ?

   *Rappelez-vous : Vous voulez mettre à jour la branche `master` pour qu'elle ait également toutes les modifications actuellement sur la branche `feature`. La commande 'git merge [nom de la branche]' prend une branche en argument à partir de laquelle elle prend des modifications. La branche pointée par HEAD (la branche actuellement vérifiée) est ensuite mise à jour pour inclure également ces modifications.*

8. Basculez sur la branche `master`.
9. Utilisez `cat` pour voir le contenu des salutations.
10. Faites la différence entre les branches.
11. Fusionnez les branches.
12. Utilisez `cat` pour voir le contenu des salutations.
13. Supprimez la branche en majuscules.

## Commandes utiles

- `git branch`
- `git branch <nom-de-branche>`
- `git branch -d <nom-de-branche>`
- `git switch`
- `git branch -v`
- `git add`
- `git commit`
- `git commit -m`
- `git merge <branche>`
- `git diff <brancheA> <brancheB>`
- `git log --oneline --graph --all`
