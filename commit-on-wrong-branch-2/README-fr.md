# Git kata: Commit sur la mauvaise branche II

## L'histoire

Vous développez une nouvelle fonctionnalité sur la branche `new-feature`. Vous avez déjà implémenté la première partie d'une fonctionnalité lorsque vous êtes informé d'un bogue critique qui doit être corrigé immédiatement sur la branche `master`.

Après la correction du bogue, vous continuez à travailler sur la nouvelle fonctionnalité. Après avoir validé la deuxième partie de la fonctionnalité, vous réalisez que vous avez effectué votre commit sur la branche `master` au lieu de la branche de la fonctionnalité.

## Configuration

1. Exécutez `source setup.sh` (ou `.\setup.ps1` dans PowerShell)

## La tâche

1. Déplacez le commit défectueux de la branche `master` vers la branche `new-feature`.
2. Comment apporteriez-vous également la correction du bogue à votre branche de fonctionnalité?

## Commandes utiles

* `git reset HEAD~1` pour déplacer la branche courante d'un pas en arrière. Cela a pour conséquence de _supprimer_ le commit le plus récent d'une branche.
* `git stash` pour sauvegarder temporairement vos modifications afin de pouvoir changer de branche.
* `git cherry-pick` pour ajouter un ensemble de modifications à partir d'un commit sur la branche actuelle.
