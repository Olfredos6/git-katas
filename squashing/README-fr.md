# Écraser les commits

Dans cette kata, je voudrais un peu nettoyer mon historique.

Les cinq commits les plus récents jouent tous avec `file.txt`, qui contient évidemment ma fonctionnalité.

Je voudrais que ces commits soient écrasés en un seul et avoir un bon message de commit (voir Informations supplémentaires).

Pendant que vous y êtes, j'aimerais vraiment que les caractères `\n` dans `file.txt` soient supprimés de l'historique.

## Configuration

1. Exécutez `source setup.sh` (ou `.\setup.ps1` dans PowerShell)

## La tâche

1. _Écrasez_ les cinq commits pertinents en un seul et rédigez un bon message de commit (voir Informations supplémentaires).
2. Comment se présente `git log` maintenant?
3. Nettoyez les caractères `\n` à l'intérieur de `file.txt` sans les ajouter à l'historique des commits.

## Commandes utiles

- `git rebase -i <référence>`
- `git add`
- `git commit --amend`

## Informations supplémentaires

### Les sept règles d'un excellent message de commit Git

Extrait de [How to Write a Git Commit Message](https://chris.beams.io/posts/git-commit/)

1. Séparez le sujet du corps par une ligne vide.
2. Limitez la ligne de sujet à 50 caractères.
3. Mettez en majuscule la ligne de sujet.
4. Ne terminez pas la ligne de sujet par un point.
5. Utilisez le mode impératif dans la ligne de sujet.
6. Enveloppez le corps à 72 caractères.
7. Utilisez le corps pour expliquer le quoi et le pourquoi plutôt que le comment.

Exemple

```MD
Résumez les changements en environ 50 caractères ou moins

Texte explicatif plus détaillé, si nécessaire. Enveloppez-le à environ 72
caractères environ. Dans certains contextes, la première ligne est traitée comme le
sujet du commit et le reste du texte comme le corps. La
ligne vide séparant le résumé du corps est cruciale (sauf
si vous omettez le corps entièrement) ; divers outils comme `log`,
`shortlog` et `rebase` peuvent être confus si vous les exécutez ensemble.

Expliquez le problème que résout ce commit. Concentrez-vous sur le pourquoi
vous apportez cette modification plutôt que sur la manière (le code l'explique).
Existet-il des effets secondaires ou d'autres conséquences inintuitives de ce
changement ? C'est l'endroit pour les expliquer.

Les paragraphes supplémentaires viennent après des lignes vides.

 - Les listes à puces sont également acceptées

 - En général, un tiret ou un astérisque est utilisé pour la puce, précédé
   d'un seul espace, avec des lignes vides entre eux, mais les conventions
   varient ici.

Si vous utilisez un gestionnaire de problèmes, ajoutez des références à ceux-ci en bas,
comme ceci :

Résout : #123
Voir aussi : #456, #789
```
