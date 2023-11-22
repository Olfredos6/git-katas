# gitkatas

## Configuration

1. Exécutez `source setup.sh` (ou `.\setup.ps1` dans PowerShell)

## Kata 5: Commit sur la mauvaise branche

Cette kata a été honteusement inspirée de [Git Katas](http://blog.schauderhaft.de/gitkata/)

Vous travaillez vraiment dur sur la branche master.
Une partie de votre travail est déjà validée. C'est à ce moment que votre patron arrive avec une demande urgente.

Étant donné que votre HEAD actuel n'est pas prêt pour la production, vous sauvegardez un commit en arrière et démarrez une nouvelle branche nommée 'quickfix'. Vous faites ce que votre patron demande et validez les modifications sur cette nouvelle branche.

C'est à ce moment que vous réalisez que vous avez créé un petit désordre avec vos branches.

Actuellement, vos commits ressemblent à ceci :

```text
         master
           |
           v
   A <---- B
   ^ \
   |  \--- C
remote     ^
           |
        quickfix
```

Mais vous voulez que cela ressemble à ceci :

```text
         remote
           |
           v
   A <---- C <---- B
                   ^
                   |
                  HEAD
```

Git en avant !

Note : comme le `B` dans la structure actuelle et dans la structure cible n'a pas le même parent, ils ne peuvent pas être littéralement le même commit.

## La tâche

1. Utilisez `git log --oneline --graph --all` pour voir toutes les branches et leurs commits.
2. Copiez `C` sur `master` avant `B` en rebasant `quickfix` sur `master`.
3. Créez une nouvelle branche (`changes-including-B`) à partir de notre `master` pour pouvoir continuer à travailler sur `B`.
4. Réinitialisez `master` sur `C`.
5. Supprimez la branche `quickfix`.
6. Poussez `master`. Vous ne pouvez pas faire cela dans l'exercice d'entraînement.
7. Vous pouvez fusionner la branche `changes-including-B` dans `master` et supprimer `changes-including-B` ou simplement basculer sur `changes-including-B` et travailler là-bas.

## Commandes utiles

- `git log --oneline --graph --all`
- `git switch <branch-name>`
- `git rebase <branch-name>`
- `git branch <branch-name>`
- `git reset --soft HEAD~`
- `git branch -d <branch-name>`
- `git merge <branch-name>`
