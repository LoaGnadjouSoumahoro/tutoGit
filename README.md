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

## Rédiger un commit

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



##Envoyer un commit sur le dépôt distant
```bash
git add .
git commit -m "Titre du commit"
git push origin main
```
