# Git Kata: Étiquetage des commits

## Configuration

1. Exécutez `source setup.sh` (ou `.\setup.ps1` dans PowerShell).

## Motivation

[Les tags](https://git-scm.com/book/en/v2/Git-Basics-Tagging) sont pratiques pour suivre les commits qui incrémentent un numéro de version. Une manière de les utiliser est en conjonction avec les branches, où l'on peut étiqueter les commits dans une branche s'ils incrémentent le numéro de version, par exemple, une branche appelée `version/1.1` peut avoir les tags `1.1.1`, `1.1.2`, etc. Les tags peuvent également être utilisés sans branches.

Il existe deux types de tags, les tags annotés et les tags non annotés. Les tags annotés peuvent contenir des informations supplémentaires, par exemple, vous pourriez ajouter des sorties de journal, en plus du nom. Outre les tags annotés, vous pouvez créer des tags non annotés qui n'ont que le nom. Dans certains cas, les tags sans annotations fonctionnent bien, car le nom du tag et les changements du commit contiennent les informations nécessaires.

## La tâche

Pour simplifier, nous travaillerons uniquement avec la branche master dans cette kata. Quelques tags sont déjà créés.

1. Voir quels tags ont été créés.
2. Faire un nouveau commit et introduire un nouveau tag annoté.
3. Nous avons fait quelques commits. Pouvez-vous ajouter un tag à un commit arbitraire ?
4. Le dépôt d'exercices contient un tag annoté. Quel est le message ?
5. Peut-être que tous les tags ne sont pas nécessaires. Supprimez-en certains.

## Commandes utiles

- `git tag`
- `git tag -d <tag>`
- `git tag --list <pattern>`
- `git push --tags <branch>`
- `git rev-parse <tag>`
- `git show`