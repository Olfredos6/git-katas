# Git Kata: Fusion à 3 Voies

## Configuration

1. Exécutez `source setup.sh` (ou `.\setup.ps1` dans PowerShell)

## La tâche

Vous vivez à nouveau dans votre propre branche, cette fois-ci nous jonglerons un peu avec les branches, pour montrer à quel point les branches sont légères dans git.

1. Créez une branche appelée `greeting` et basculez dessus.
2. Modifiez le fichier `greeting.txt` pour y insérer votre salutation préférée.
3. Ajoutez le fichier `greeting.txt` à la zone de transit.
4. Faites un commit.
5. Revenez à la branche `master`.
6. Créez un fichier README.md avec des informations sur ce dépôt.
7. Ajoutez le fichier README.md à la zone de transit et faites le commit.
8. Quelle est la sortie de `git log --oneline --graph --all` ?
9. Faites la différence entre les branches.
10. Fusionnez la branche `greeting` dans `master`.
11. Quelle est la sortie de `git log --oneline --graph --all` maintenant ? Observez le commit de fusion supplémentaire créé avec le message "Merge branch 'greeting'".

## Commandes utiles

- `git branch`
- `git branch <nom-de-branche>`
- `git branch -d <nom-de-branche>`
- `git switch <nom-de-branche>`
- `git switch -c <nom-de-branche>`
- `git branch -v`
- `git add`
- `git commit`
- `git commit -m`
- `git merge <brancheA> <brancheB>`
- `git diff <brancheA> <brancheB>`
- `git log --oneline --graph --all`
