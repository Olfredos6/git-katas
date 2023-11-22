# Git katas: Réinitialiser Git

Nous pouvons manipuler l'historique de manière très poussée. Nous devrions seulement jouer avec notre historique local. Les commits publiques doivent être considérés comme immuables.

Nous utilisons `reset` pour désélectionner des changements, mais nous pouvons également faire beaucoup d'autres choses différentes.

## Configuration

1. Exécutez `source setup.sh` (ou `.\setup.ps1` dans PowerShell)

## Tâche

1. À quoi ressemble votre répertoire de travail ?
2. À quoi ressemble votre log ? À quoi ressemble votre zone de transit ?
3. Essayez d'exécuter `git reset --soft HEAD~1`.
4. Que se passe-t-il dans votre répertoire de travail, votre journal et votre zone de transit ?
5. Exécutez `git reset --mixed HEAD~1`.
6. Que se passe-t-il dans votre répertoire de travail, votre journal et votre zone de transit ?
7. Exécutez `git reset --hard HEAD~1`.
8. Que se passe-t-il dans votre répertoire de travail, votre journal et votre zone de transit ?
9. Essayez maintenant d'utiliser `git revert HEAD~1`.
10. Que se passe-t-il dans votre répertoire de travail, votre journal et votre zone de transit ?

## Commandes utiles

- `git log --oneline`
- `git commit --amend`
- `git status`
- `git reset --soft`
- `git reset --mixed`
- `git reset --hard`
- `git revert`

## Explication supplémentaire

Ce qui suit est tiré de la section Récapitulation de [https://git-scm.com/book/en/v2/Git-Tools-Reset-Demystified] (texte en Anglais).
La commande `reset` écrase ces trois arbres dans un ordre spécifique, s'arrêtant lorsque vous lui dites de le faire :

1. Déplacer là où pointe la tête de la branche (s'arrêter ici si --soft)
2. Faire en sorte que la zone de transit ressemble à la tête (s'arrêter ici sauf si --hard)
3. Faire en sorte que le répertoire de travail ressemble à la zone de transit
