# gitkatas

## Kata 7: Réorganisation de l'historique

Les commits ici ont clairement été faits par un fou :sweat_smile:.
Malheureusement, ils contiennent en réalité des informations utiles - c'est juste que l'historique est étrange.
Vous devez arranger cela de manière à ce que notre `git log` soit génial !

## Configuration

1. Exécutez `source setup.sh` (ou `.\setup.ps1` dans PowerShell)

## Tâche

Réorganisez l'historique de manière à ce qu'il ait réellement du sens - ajoutez les fichiers dans l'ordre qui correspond à leur nom.

1. Utilisez `git log --oneline --graph` pour voir les commits.
2. Essayez également `git reflog` pour voir les commits. `git reflog` est par défaut équivalent à `git reflog show`, qui est un alias de `git log -g --abbrev-commit --pretty=oneline`.
3. Utilisez `git rebase -i <après-ce-commit>` pour réorganiser les commits. Il y a des commentaires dans le fichier que vous éditez qui expliquent les commandes disponibles.
4. Utilisez `git log --oneline --graph` pour voir le résultat

### Commandes utiles

- `git rebase -i <après-ce-commit>`
- `git log --oneline --graph`
- `git reflog`
