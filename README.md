# Création d'un dépot GIT

## Création d'un dépot GIT en local

Dans la console, initialisation du dépot: 

```bash
git init
´´´
## visualisation de l'état de GIT 
```bash
git status
´´´

### Pour voir les fichiers et dossiers Unix 

```bash
ls -a
```

## Pour ajouter un fichier à la  future sauvegarde 
```bash
git add README.md
```
## Pour effectuer la sauvegarde
Les fichiers en attente de sauvegarde sont en vert 
les fichiers non suivi sont en rouges
seul les fichiers en **staging** seront sauvés
```bash
git commit -m"Message du commit"
```
Un commit est une sauvegarde, on peut y accéder avec un `git log` (affichage 
des identifiants des sauvegardes
 et `git show`(sans paramètres, affichage du dernier)

## Pour ajouter tous les fichiers en staging
```bash
git add.
```
## Ajout d'un serveur distant
