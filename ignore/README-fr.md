# Git Kata: Ignorer les bases

Nous allons travailler un peu avec le fichier `.gitignore` dans ce kata.
Dans ce fichier, vous pouvez spécifier à la fois les extensions de fichiers et les structures de dossiers que vous ne voulez pas que Git suive.
Vous pouvez toujours utiliser `git add` pour les fichiers et dossiers qui sont ignorés dans le fichier `.gitignore`.

Nous travaillerons également avec `git rm`, qui est la commande de suppression de Git. `git rm` fait exactement la même chose que supprimer un fichier de votre répertoire de travail, puis mettre en scène ce changement en utilisant `git add nomfichier` sur le fichier qui vient d'être supprimé.
Parfois, vous ajoutez un fichier par accident qui n'était pas destiné à Git, par exemple des fichiers binaires, des fichiers de classe, etc.

Si vous voulez indiquer à Git qu'un fichier doit être supprimé de Git, mais que vous voulez toujours le conserver dans votre répertoire de travail, utilisez `git rm --cached` pour émettre une commande de suppression dans l'index, mais pas dans votre répertoire de travail.

## Configuration

1. Exécutez `source setup.sh` (ou `.\setup.ps1` dans PowerShell)

## La tâche

1. Créez un fichier avec le nom `foo.s`
2. Quelle est la sortie de `git status` ?
3. Créez un fichier `.gitignore` dans votre répertoire de travail contenant `*.s`
4. Quelle est la sortie de `git status` ?
5. Validez le fichier `.gitignore`
6. Validez `file1.txt`
7. Ajoutez les fichiers `txt` à `.gitignore` en ajoutant une ligne dans le fichier contenant `*.txt`
8. Que nous indique `git status` ?
9. Modifiez `file1.txt`
10. Que nous indique `git status` ? Pourquoi le fichier a-t-il été suivi même si l'extension `txt` est dans le fichier d'ignorance ?
11. Créez un autre fichier texte `file2.txt` dans le référentiel, à quoi ressemble `git status` maintenant ? Pourquoi n'est-il pas suivi ?
12. Mettez en scène la suppression de `file1.txt` avec la commande `git rm --cached`
13. Que nous indique `git status` ?
14. Créez un nouveau fichier appelé `file3.txt` et ajoutez la ligne `!file3.txt` à `.gitignore`. (Voir la _note_ ci-dessous)
15. Que nous indique `git status` ? Pouvez-vous penser à un cas d'utilisation pour suivre un fichier bien que l'extension soit ignorée ?

## Note

Si vous utilisez `zsh` au lieu de `bash` (par défaut sur Mac et certaines distributions Linux), alors `echo "!file3.txt" >> .gitignore` échouera en raison de l'expansion du shell. Utilisez un éditeur pour modifier le fichier ou échappez le `!` par exemple `echo "\!file3.txt" >> .gitignore`

## Commandes utiles

- `git rm`
- `git add`
- `git commit`
- `git commit -m`
- `git rm --cached`

## Alias

Vous pouvez configurer des alias comme ceci :
`git config --global alias.lol 'log --oneline --graph --all'`
Cela pourrait vous être utile.
