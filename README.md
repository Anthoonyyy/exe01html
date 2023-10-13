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
le -a permet d'afficher les fichiers cachés

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

## Pour retirer un fichier du staging 
```bash
git restore --staged README.md
```

## Ajout d'un serveur 
Nous allons utiliser un dépôt que l'on va créer sur github.com
après connexion. Comme c'est un travail personel, son URL sera de ce type
https://github.com/Username/Le nomduprojet
 
Nous créons un new repository, puis nous copions la clé SSH :
 
git@github.com:Anthoonyyy/exe01html.git

Nous retournons dans notre console:
```bash
git remote add origin git@github.com:Anthoonyyy/exe01html.git
```
Pour voir si ca a fonctionner :
```bash
git remote -v
```
## Envoi du projet 
```bash
git push origin main
```
## Récupération du projet 
Si on souhaite récuperer que le `.git`(donc l'historique sans les fichiers)

```bash
git fetch origin main
```
Si on souhaite récupérer toute la branche `main`

```bash
git pull origin main
```
Si on a effectué des modifications en local non voulue empêchant la récupération des fichiers.(`merge error`).

On peut utiliser un `git stash`pour faire une pseudo sauvegarde et revenir au dernier commit avant de refaire un 
`git pull`

