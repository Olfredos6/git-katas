"# Git Kata : Commit Basique
Cette kata vous initiera aux commandes `git add` et `git commit`.

C'est une kata très introductive. Si vous avez déjà utilisé `git status`, `git log --oneline --graph`, `git add` et `git commit` de manière approfondie, vous pouvez probablement la sauter.

Vous pouvez regarder le bas de ce fichier si vous n'avez pas encore effectué la configuration de base de Git.

## Configuration :

1. Exécutez `source setup.sh` (ou `.\setup.ps1` dans PowerShell)

## La tâche

1. Utilisez `git status` pour voir sur quelle branche vous vous trouvez.
2. À quoi ressemble `git log` ?
3. Créez un fichier.
4. À quoi ressemble la sortie de `git status` maintenant ?
5. Ajoutez le fichier à la zone de transit.
6. Comment se présente maintenant `git status` ?
7. `commit` le fichier dans le référentiel.
8. Comment se présente maintenant `git status` ?
9. Modifiez le contenu du fichier que vous avez créé précédemment.
10. À quoi ressemble `git status` maintenant ?
11. Ajoutez la modification du fichier.
12. À quoi ressemble `git status` maintenant ?
13. Modifiez à nouveau le fichier.
14. Faites un `commit`.
15. À quoi ressemble le `status` maintenant ? Et le `log` ?
16. Ajoutez et faites un commit de la dernière modification.

## Commandes utiles
- `git add`
- `git commit`
- `git commit -m "Mon message de commit"`
- `git log`
- `git log -n 5`
- `git log --oneline`
- `git log --oneline --graph`
- `touch nomdufichier` pour créer un fichier (ou `sc nomdufichier ''` dans PowerShell)
- `echo contenu > fichier` pour écraser le fichier avec du contenu (ou `sc nomdufichier 'contenu'` dans PowerShell)
- `echo contenu >> fichier` pour ajouter du contenu au fichier (ou `ac nomdufichier 'contenu'` dans PowerShell)

## Configuration Initiale de Git
1. `git config --global user.name "John Doe"`
2. `git config --global user.email "johndoe@example.com"`

Pour les amateurs de vim :
- `git config --global core.editor nano`

Pour les utilisateurs de Windows :
- `git config --global core.editor notepad`

Autres options d'éditeur :
- `git config --global core.editor "atom --wait"`
- `git config --global core.editor "code --wait"`
- `git config --global core.editor "'C:/Program Files/Notepad++/notepad++.exe' -multiInst`"