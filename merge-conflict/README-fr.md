# Git Kata: Conflit de Fusion

## Configuration

1. Exécutez `source setup.sh` (ou `.\setup.ps1` dans PowerShell)

## La tâche

Dans cette kata, Git ne peut pas comprendre comment fusionner le contenu ajouté sur `merge-conflict-branch1` avec le contenu sur `master`.

Les deux changements doivent être présents dans `master` lorsque vous avez terminé.

1. Utilisez `git merge` pour apporter les changements de `merge-conflict-branch1` dans `master`.
2. Que rapporte maintenant `git status` ?
3. Résolvez le conflit avec votre éditeur préféré.
4. Suivez les instructions dans `git status` pour terminer la fusion.
5. Que montre `git log --oneline --graph` ?

## Commandes pertinentes

- `git merge`
- `git status`
- `git add`
- `git commit`
- `git log --oneline --graph`
