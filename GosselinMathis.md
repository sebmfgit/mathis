# Voici le répertoire des commandes Git utilisées pour le TP test

## Initialisation

```shell
mkdir tptest
git init
```
## Resolution des Problèmes : 
```shell
git clone "https://github.com/sebmfgit/mathis"
cd mathis
```
## Création de la brache
```shell
git branch index
git push origin index
git checkout index
```

## Envoie du premier commit de l'index
```shell
git add "index.html"
git commit -m "Premier dépot de la page index"
git push origin index
```

## Récuperation des branches des collaborateurs  : 
```shell
git fetch --all
git checkout css
nano style.css
nano stylec.css
touch stylem.css
nano stylem.css
```


## Envoie des modifications aux braches respectives


### CSS :

Modification des fichiers styles pour l'index et contact, et l'ajout d'un nouveau pour media.

```shell
git add style.css stylec.css
git commit -m "Modification des feuilles de styles pour la page index et contact"
git push -u origin css

touch stylem.css
nano stylem.css
git add stylem.css
git commit -m "Ajout de styles de la page media"
git push -u origin css
```

### Media :

Modification du code html et ajout des images

```shell
git checkout media
nano media.html
git add media.html img.jpg
git commit -m "Modification du code media et ajout de l'image correspondante"
git push -u origin media
```
transfaire de l'image depuis la machine hôte grace à WinSCP

### Contact :

Modification du code html 

```shell
git checkout contact
git nano contact.html

git add contact.html
git commit -m "Modification du code contact"
git push -u origin contact
```

### Index :

Modification du code html 

```shell
git checkout index
git nano index.html

git add index.html
git commit -m "Modification du code index"
git push -u origin index
```

## Merge :

Création du branche "Final" avec de merge sur le main

```shell
git branch final
git checkout final
git push origin final

git merge media

git merge contact

git nano contact.html
git commit -m "résolution des conflits"
git push origin final

git merge css

git merge index
git log final..index --oneline

git add index img2.jpg
git commit -m "Problème avec le merge pour index.html donc commit manuel"
git push -u origin final

```

## Merge final sur le main

```shell
git checkout main
git pull 

git merge final
```

