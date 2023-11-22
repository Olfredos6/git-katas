
# gitkatas

## Rébase interactif avancé

Vous avez travaillé sur une nouvelle fonctionnalité appelée Hello World.
Cette fonctionnalité est complète avec à la fois la documentation et les tests unitaires, mais il y a quelques problèmes.
L'historique semble vraiment désordonné, avec beaucoup de petites étapes à moitié terminées, et il y a des éléments inclus qui n'auraient jamais dû l'être.

Vous devez résoudre cela de manière à ce que votre `git log` soit propre !

Pour ce faire, nous utiliserons notre bon ami `git rebase --interactive`.

Heureusement, nous avons une étiquette de version `v0.0` juste avant le début de la fonctionnalité.

Comme il s'agit d'un exercice avancé, il n'y a pas d'étapes spécifiques à suivre et pas de solution unique.

## Configuration

1. Exécutez `source setup.sh` (ou `.\setup.ps1` dans PowerShell)

## Tâche

1. Explorez le référentiel et l'historique pour comprendre ce qui s'est passé.
2. Utilisez `git rebase --interactive v0.0` pour vous permettre de modifier la "recette" pour l'ensemble du développement de la fonctionnalité.
3. Nettoyez l'historique de manière à ce qu'il ait réellement du sens. Essayez d'utiliser autant de "fonctionnalités" de rebase (par exemple, reword, squash, fixup, drop) que possible. Vous décidez vous-même si vous voulez tout réécrire d'un coup, ou appliquer quelques modifications d'abord, puis exécuter un nouveau `git rebase --interactive v0.0` pour continuer le nettoyage.

### Commandes utiles

- `ls -l`                 # lister les fichiers
- `tail -n +1 *`          # afficher le contenu de tous les fichiers
- `git log --oneline`     # afficher l'historique
- `git log --stat`        # historique des fichiers modifiés
- `git log --patch`       # historique avec diff
- `git rebase -i <ref>`   # exécuter le rébase interactif jusqu'à <ref>
