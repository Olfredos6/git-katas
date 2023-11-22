# Git Katas: Sous-modules

Les sous-modules sont une manière d'intégrer d'autres dépôts Git dans le vôtre, en conservant un pointeur vers son `origin`. Cela vous permet de récupérer directement les modifications du code source, ainsi que de les _pousser_ en arrière.

## Configuration

1. Exécutez `source setup.sh` (ou `.\setup.ps1` dans PowerShell)

> NOTE : Si vous exécutez setup.sh sur Windows, vous pouvez rencontrer des problèmes en sourçant le script de configuration. À la place, exécutez `./setup.sh`, et les dossiers seront créés correctement.

## La tâche

Après avoir exécuté le script de configuration, vous vous retrouverez avec trois dépôts à l'intérieur du dossier `exercise`.

* Un dépôt `remote`. Il s'agit du dépôt "remote" qui existerait normalement sur votre hébergeur Git préféré, par exemple github.com.
* Un dépôt `component` cloné depuis `remote`.
* Un dépôt `product`.

Allez dans le dépôt `product`.

1. Ajoutez le composant en tant que sous-module du produit en exécutant `git submodule add ../remote include`.
2. À quoi ressemble votre répertoire de travail?
3. La commande `git status` affiche-t-elle ce à quoi vous vous attendez?
4. Que se passe-t-il si vous vous déplacez vers `include`?
5. Exécutez `git diff --staged` dans `product`. Où pouvez-vous trouver l'ID de commit indiqué dans la ligne `+Subproject commit ...`?
6. Validez les modifications dans le dépôt `product`.

   Allez dans le dépôt `component`.

7. Sait-il qu'il est utilisé en tant que sous-module?
8. Apportez une modification au dépôt `component`, puis faites `git commit` et `git push`.

   Retournez dans le dépôt `product`.

9. Les commandes `git status` ou `git submodule foreach 'git status'` vous disent-elles quelque chose sur ce nouveau commit?
10. Allez dans le répertoire `include` et faites `git pull` pour obtenir la dernière version.
11. Vérifiez que la modification du dépôt `component` est disponible dans `include`.
12. Retournez dans le répertoire `product`. Quel est l'état actuel de votre dépôt de produits? Examinez également avec `git diff`.
13. Allez dans votre dossier `include`. Apportez une modification et effectuez un `push` vers son origine.

    Retournez dans le répertoire `exercise`. Nous allons créer un clone du produit pour illustrer comment les sous-modules dans un clone doivent être initialisés.

14. Exécutez `git clone product product_alpha`.
15. Allez dans le répertoire `product_alpha`, à quoi ressemble votre répertoire de travail, que dit le journal et que contient le répertoire `include`?
16. Exécutez `git submodule init`, à quoi ressemble votre répertoire `include` maintenant?
17. Exécutez `git submodule update`, à quoi ressemble votre répertoire `include` maintenant?
    (* Remarque : vous pouvez combiner les deux étapes précédentes en exécutant `git submodule update --init`)
18. La dernière modification du composant est-elle disponible dans `include`?

    Retournez dans le dépôt `product`.

19. Validez les modifications dans le dépôt `product`. Oubliez de pousser les modifications pour le moment ;-)

    Allez dans le dépôt `product_alpha`. Assurons-nous d'avoir les dernières modifications du produit.

20. Exécutez `git submodule update`.
21. La dernière modification du composant est-elle disponible dans `include`?
22. Examinez la sortie de `git submodule status`. Comparez l'ID de commit avec le dépôt `component`.
23. Exécutez `git submodule update --remote`.
24. La dernière modification du composant est-elle disponible dans `include`?
25. Examinez la sortie de `git submodule status`. Comparez l'ID de commit avec le dépôt `component`.

En tant qu'exercice bonus, essayez de représenter tout cet exercice sur papier!

## Commandes utiles

```shell
git diff [--cached] --submodule
git log -p --submodule
```
