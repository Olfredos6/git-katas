# Git kata: Modification de commits

Lorsque nous travaillons, nous effectuons beaucoup de commits. Parfois, nous oublions quelque chose d'évident que nous voulons corriger rapidement. `git commit --amend` nous permet de le faire - manipuler le dernier commit que nous avons fait. Vous pouvez utiliser `git log -p` ou `git show` pour inspecter le contenu des commits et les modifications de fichiers qui ont été ajoutées aux commits.

## Configuration

1. Exécutez `source setup.sh` (ou `.\setup.ps1` dans PowerShell)

## La tâche

1. Que nous dit `git status` ?
2. Que nous dit `git log -p` ?
3. Mettez en scène l'ajout de bar.txt.
4. Exécutez `git commit --amend`.
5. Qu'est-ce qui s'est passé ? Que nous dit `git log -p` ?
6. Que se passe-t-il si vous exécutez à nouveau `git commit --amend` ?

## Commandes utiles

- `git add`
- `git log --oneline --graph`
- `git log -p`
- `git show`
- `git commit --amend`
