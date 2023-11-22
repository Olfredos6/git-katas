# Git Kata : Staging de Base

Cette kata examinera la zone de transit de git.

Dans git, nous travaillons avec trois zones différentes :

* Le répertoire de travail où vous apportez vos modifications
* La zone de transit où toutes les modifications que vous avez ajoutées via `git add` resteront
* Le référentiel où chaque commit aboutit, créant ainsi votre historique. Pour mettre vos modifications en attente ici, vous utilisez la commande `git commit`.

Un fichier peut avoir des modifications à la fois dans le répertoire de travail et dans la zone de transit.
Ces modifications ne doivent pas nécessairement être les mêmes.

Nous utiliserons également `git restore` pour restaurer les modifications en attente d'un fichier, et `git checkout` pour revenir à un état précédent d'un fichier.

## Configuration

1. Exécutez `source setup.sh` (ou `.\setup.ps1` dans PowerShell)

## La tâche

Vous vivez dans votre propre référentiel. Il y a un fichier appelé `file.txt`.

1. Quel est le contenu de `file.txt` ?
2. Écrasez le contenu de `file.txt` : `echo 2 > file.txt` pour changer l'état de votre fichier dans le répertoire de travail (ou `sc file.txt '2'` dans PowerShell)
3. Que vous dit `git diff` ?
4. Que vous dit `git diff --staged` ? Pourquoi est-ce vide ?
5. Exécutez `git add file.txt` pour mettre en attente vos modifications depuis le répertoire de travail.
6. Que vous dit `git diff` ?
7. Que vous dit `git diff --staged` ?
8. Écrasez le contenu de `file.txt` : `echo 3 > file.txt` pour changer l'état de votre fichier dans le répertoire de travail (ou `sc file.txt '3'` dans PowerShell).
9. Que vous dit `git diff` ?
10. Que vous dit `git diff --staged` ?
11. Expliquez ce qui se passe
12. Exécutez `git status` et observez que `file.txt` est présent deux fois dans la sortie.
13. Exécutez `git restore --staged file.txt` pour désélectionner la modification.
14. Que vous dit `git status` maintenant ?
15. Mettez la modification en attente et faites un commit.
16. À quoi ressemble le log ?
17. Écrasez le contenu de `file.txt` : `echo 4 > file.txt` (ou `sc file.txt '4'` dans PowerShell)
18. Quel est le contenu de `file.txt` ?
19. Que nous dit `git status` ?
20. Exécutez `git restore file.txt`
21. Quel est le contenu de `file.txt` ?
22. Que nous dit `git status` ?

## Commandes utiles

- `git add`
- `git commit`
- `git commit -m "Mon message de commit court et paresseux"`
- `git log`
- `git log -n 5`
- `git log --oneline`
- `git log --oneline --graph`
- `git restore --staged`

## Alias

Vous pouvez configurer des alias de la manière suivante :
`git config --global alias.lol 'log --oneline --graph --all'`
Cela peut vous être utile.
