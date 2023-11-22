# Git-Katas(fr)

Ce dépôt est un fork actif de [eficode-academy/git-katas](https://github.com/eficode-academy/git-katas). Le but de ce fork est principalement de fournir une version traduite en français de ce fabuleux travail.

## Configuration

![Démarrage rapide](/images/quickstart.gif)

Avant de commencer, assurez-vous d'avoir Git installé et prêt à être utilisé. Si vous n'êtes pas sûr que votre environnement soit configuré et prêt, veuillez consulter [configure-git](configure-git/README.md) pour vous en assurer.

- Clonez ce dépôt
- Accédez au dossier dans lequel vous souhaitez résoudre un exercice
- Exécutez le script `setup.sh`
- Consultez le fichier README-fr.md dans ce dossier pour obtenir une description de l'exercice.

## Vue d'ensemble

"## Aperçu des exercices de Git Kata

## Git Katas de base dans l'ordre suggéré

1. [basic-commits](basic-commits/README.md) - Création très basique de commits.
2. [basic-staging](basic-staging/README.md) - Interaction avec la zone de transit (index).
3. [basic-branching](basic-branching/README.md) - La première incursion dans le branching.
4. [ff-merge](ff-merge/README.md) - Un tour autour des fusions les plus triviales.
5. [3-way-merge](3-way-merge/README.md) - Une fusion de base impliquant plusieurs branches divergentes.
6. [merge-conflict](merge-conflict/README.md) - Une fusion de base entre des branches divergentes avec des ensembles de changements incompatibles (mais simples).
7. [merge-mergesort](merge-mergesort/README.md) - Un conflit de fusion avec du code réel.
8. [rebase-branch](rebase-branch/README.md) - Utilisation du rebase comme alternative à la fusion.
9. [basic-revert](basic-revert/README.md) - Utilisez revert pour annuler un changement.
10. [reset](reset/README.md) - Reset est une commande puissante et légèrement dangereuse si vous ne savez pas ce que vous faites. Parcourez les trois modes de reset ici.
11. [basic-cleaning](basic-cleaning/README.md) - Nettoyer l'espace de travail.
12. [amend](amend/README.md) - Modifier les commits précédents.
13. [reorder-the-history](reorder-the-history/README.md) - Nous avons peut-être créé nos commits dans un ordre suboptimal, pratiquez pour résoudre ce scénario ici.
14. [squashing](squashing/README.md) - Beaucoup de petits commits sont bons lorsque vous travaillez localement, mais pour partager votre code, il pourrait être plus bénéfique de livrer vos changements de code en grands ensembles. Allez ici pour expérimenter cela. Rédigez un bon commit.
15. [advanced-rebase-interactive](advanced-rebase-interactive/README.md) - Pratiquez l'utilisation des commandes de rebase interactif.
16. [basic-stashing](basic-stashing/README.md) - La première incursion dans le stashing.
17. [ignore](ignore/README.md) - Les bases de l'utilisation du fichier `.gitignore`. Et utilisation de `git rm`.
18. [submodules](submodules/README.md) - Les sous-modules sont détestés par beaucoup. Parcourez cet exercice pour comprendre de quoi il s'agit.
19. [git-tag](git-tag//README.md) - Les tags sont pratiques pour suivre les commits qui incrémentent un numéro de version. Dans cet exercice, vous listerez, ajouterez et supprimerez des tags.

## Katas résolvant des problèmes standards

1. [commit-on-wrong-branch](commit-on-wrong-branch/README.md) - Si nous mettons accidentellement des commits non poussés sur la mauvaise branche, comment les déplacer efficacement vers une autre branche avant notre travail sur cette branche.
2. [commit-on-wrong-branch-2](commit-on-wrong-branch-2/README.md) - Un autre exercice sur ce qu'il faut faire si vous avez accidentellement commis sur la mauvaise branche.
3. [reverted-merge](reverted-merge/README.md) - Nous annulons une fusion, mais après l'ajout de correctifs à la branche fusionnée, nous voulons les changements de la fusion et les nouveaux correctifs.
4. [save-my-commit](save-my-commit/README.md) - Si vous supprimez accidentellement ou délibérément un commit, allez ici pour essayer de le sauver. Vous utiliserez le reflog.
5. [detached-head](detached-head/README.md) - Git se plaint que vous êtes dans un état "You are in 'detached HEAD' state". Que faites-vous?

## Katas sur les fonctionnalités avancées

1. [git-attributes](git-attributes/README.md) - Le fichier .gitattributes vous permet de spécifier comment git gère les fichiers, tels que les sauts de ligne dans les fichiers texte ou comment différencier un fichier binaire.
2. [Bad-commit](bad-commit/README.md) - Utilisation de `git bisect` pour trouver un mauvais commit.
3. [bisect](bisect/README.md) - Un autre kata utilisant `git bisect`.
4. [pre-push](pre-push/README.md) - Un exercice rapide sur l'utilisation des crochets Git.
5. [Investigation](investigation/README.md) - Découvrez ce qui se passe dans un référentiel Git, comprenez à quoi cela ressemble sous le capot.
6. [Objects](objects/README.md) - Un petit exercice sur les entrailles de Git.
7. [merge-driver](merge-driver/README.md) - Définition d'un pilote de fusion personnalisé.
8. [rebase-exec](rebase-exec/README.md) - Exécutez des tests sur chaque commit en utilisant `git rebase --exec`.
