# Git Kata: Stash basique

## Configuration

1. Exécutez `source setup.sh` (ou `.\setup.ps1` dans PowerShell)

## La tâche

Vous travaillez sur votre projet. Vous avez mis en scène certains changements et avez également quelques changements non mis en scène.
Soudain, vous êtes informé qu'un bogue a atteint la production. Vous allez mettre en réserve votre travail, corriger le bogue et revenir à votre travail initial.

1. Explorez le dépôt
   1. Quel travail avez-vous dans le répertoire de travail ?
   2. Quel travail avez-vous mis en scène ?
   3. À quoi ressemble l'historique des commits ?
   > *Remarquez que file.txt a des changements mis en scène (c'est-à-dire des changements dans l'index) et des changements non mis en scène (des changements dans le répertoire de travail)*
2. Utilisez `git stash` pour mettre en réserve votre travail actuel.
   1. Maintenant, quel travail avez-vous dans le répertoire de travail ?
   2. Quel travail avez-vous mis en scène ?
   3. À quoi ressemble l'historique des commits ?
   4. À quoi ressemble la liste des mises en réserve (`stash`) ?
3. Corrigez les fautes de frappe dans bug.txt sur la branche master et effectuez votre commit.
4. Maintenant, pour revenir à votre travail, appliquez la mise en réserve sur la branche master.
   1. Quel travail avez-vous dans le répertoire de travail ?
   2. Quel travail avez-vous mis en scène ?
   > *Oops. Tous nos changements ne sont maintenant plus mis en scène. Cela peut être indésirable et inattendu.*
5. Annulez nos changements avec `git reset --hard HEAD`. C'est une commande dangereuse car elle supprimera définitivement des fichiers de votre index et de votre répertoire de travail, mais nous avons nos changements en sécurité dans la mise en réserve, donc tout va bien. Consultez le kata sur [reset](reset/README.md) si vous n'êtes pas sûr de ce qui se passe ici.
6. Appliquez la mise en réserve sur master avec l'option `--index`.
   1. Quel travail avez-vous dans le répertoire de travail ?
   2. Quel travail avez-vous mis en scène ?
   > *Ok, de retour à où nous étions !*
7. Nous n'aurons plus besoin de la mise en réserve. Supprimez-la.
   1. À quoi ressemble la liste des mises en réserve (`stash`) ?
   2. À quoi ressemble l'historique des commits ?

## Commandes utiles

- `git status`
- `git status -s`
- `git diff`
- `git diff master`
- `git stash`
- `git stash list`
- `git stash apply`
- `git stash apply --index`
- `git stash drop`
- `git log --oneline --all --graph`
- `git commit`
- `git add`
