# Cheat-sheet: Git

Ici vous trouverez les commandes git que vous pourriez utiliser pour ce projet :


- [Cheat-sheet: Git](#cheat-sheet-git)
  - [Connexion à un repo distant](#connexion-à-un-repo-distant)
  - [Cloner un repo](#cloner-un-repo)
  - [Ajouter un fichier](#ajouter-un-fichier)
  - [Retirer un fichier](#retirer-un-fichier)
  - [Commit](#commit)
  - [Push](#push)
  - [Pull](#pull)
  - [Créer une branche](#créer-une-branche)
  - [Changer de branche](#changer-de-branche)
  - [Voir les branches](#voir-les-branches)
  - [Fusionner une branche](#fusionner-une-branche)
  - [Supprimer une branche](#supprimer-une-branche)
  - [Voir les commits](#voir-les-commits)
  - [Voir les différences](#voir-les-différences)



## Connexion à un repo distant
[Lire la doc](https://docs.github.com/en/get-started/quickstart/set-up-git)

## Cloner un repo
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

## Retirer un fichier
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
Par défaut, la branche est `main` ou `master`

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

