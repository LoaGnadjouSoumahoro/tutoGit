#Document du tuto GitHub avec Git

##Initialisation du dépôt

```bash
git init
git remote add origin SSH_REPO
```

## Infos sur les commits

```bash
git log
git show
```

## Rédiger un commit (bonne practique)

```Titre du commit

Drescription de notre commit avec des informations du projet
```

```bash
git commit
i
:wq

```

git commit ouvre un editeur de texte en ligne de command.

i pour insérer des infos dans l'editeur

:wq permet de sortir de l'éditeur de commande. Il faut l'écrire en dernière ligne

## Annuler un Add

```bash
git restore --staged . OU NOM_DES_FICHIER_DU_ADD_QUE_ON_VEUT_SUPPRIMER
```

La suppression du add peut se faire si on n'a pas fait de commit

## Envoyer un commit sur le dépôt distant

```bash
git add .
git commit -m "Titre du commit"
git push origin main
```

## Connaitre les branches

```bash
git branch
```

## git Merge

Si on est sur Develop et on veux mettre le travail de develop sur main:
deplacer le header sur main

```bash
git checkout main
git merge develop
```

les infos en plus de develop sont sur main. Mais tous ses modifications se sont opérés en local. Pour modifier dans le répository distant il faut faire

```bash
git push origin main
```

Pour ls bonnes pratiques, on va intégrer la notion de revue de code. Pour cela, on va créer une branche, faire des modifications, les envoyer sur le dépot distant, puis créer une pull request pour demender une revue de code.

## Création d'une Branche

```bash
git checkout -b NOM_BRANCH
```
