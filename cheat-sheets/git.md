# Cheat-sheet: Git

Ici vous trouverez les commandes git que vous devriez utiliser pour ce projet :


## Connection à un repo distant
[Lire la doc](https://docs.github.com/en/get-started/quickstart/set-up-git)

## cloner un repo
```bash
git clone <url>
```

## Ajouter un fichier
```bash
git add <file>
```
pour ajouter tous les fichiers modifiés :
```bash
git add .
```

## retirer un fichier
```bash
git rm <file>
```

## Commit
```bash
git commit -m "<message>"
```
Si vous ne mettez pas de `-m "message"` git ouvrira un éditeur de texte pour que vous puissiez écrire votre message.

## Push
```bash
git push origin <branch>
```
par défaut la branche est `main` ou `master`

## Pull
```bash
git pull origin <branch>
```

## Créer une branche
```bash
git checkout -b <branch>
```

## Changer de branche
```bash
git checkout <branch>
```

## Voir les branches
```bash
git branch
```

## Fusionner une branche
```bash
git merge <branch>
```

## Supprimer une branche
```bash
git branch -d <branch>
```

## Voir les commits
```bash
git log
```

## Voir les différences
```bash
git diff
```

