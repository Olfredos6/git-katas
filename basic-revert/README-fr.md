# Git Kata: Revertir de base

## Configuration

1. Exécutez `source setup.sh` (ou `.\setup.ps1` dans PowerShell)

## La tâche

Dans cette tâche, quelques changements se sont glissés, que nous aimerions annuler. Notre historique est public, nous ne pouvons donc pas simplement le modifier. Nous devons plutôt utiliser `revert` pour supprimer les changements indésirables de manière sûre.

1. Utilisez `git log --oneline` pour examiner l'historique.
2. Utilisez `cat` pour afficher le contenu de `greeting.txt`.
3. Utilisez `git revert` sur le commit le plus récent pour supprimer les changements ajoutés par le dernier commit.
4. Utilisez `git log --oneline` pour afficher l'historique.
5. La commande de revert a-t-elle ajouté ou supprimé un commit ?
6. Utilisez `cat` pour afficher le contenu de `greeting.txt`.
7. Utilisez `ls` pour voir le contenu de l'espace de travail.
8. Utilisez `git log --oneline` pour trouver le SHA(identifiant) du commit qui a ajouté des informations d'identification au référentiel.
9. Utilisez `git revert` pour annuler le commit qui a ajouté les informations d'identification.
10. Utilisez `git log --oneline` pour afficher l'historique.
11. Utilisez `ls` pour voir le contenu de l'espace de travail.
12. Combien de commits ont été ajoutés ou modifiés par le dernier revert ?
13. Utilisez `git show` avec le SHA du commit que vous avez revert pour voir que le fichier d'informations d'identification est toujours dans l'historique.
14. Comme vous avez maintenant annulé le fichier d'informations d'identification, il est supprimé de votre répertoire de travail. Est-il également supprimé de Git ?

## Commandes utiles

- `git revert <référence>`
- `git log --oneline`
- `git show <référence>`
