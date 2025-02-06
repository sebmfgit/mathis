### ici vous trouverez toute les actions que j'ai réaliser dans le tp
```shell
cd /home
cd hgz/
cd Documents/
mkdir tpgit
cd tpgit
git init 
git remote add origin https://github.com/sebmfgit/mathis.git
git pull origin main
git branch
```

## une partie test afin de verifier que le push fonctionne, et je creer la branche
```shell
git branch css
git branch
git chechout css

touch testantoine.txt
nano testantoine.txt
git add testantoine.txt
git commit -m "test"
git config user.email "antoine.haugazeau@efrei.net"
git config user.name "gearpimento"
git push -u origin css
```
## Cela ayant fonctionner maintenant je fais la meme chose avaec le vrai fichier style.css, j'en profite pour récuperer les branches de mes camarade.
```shell
git pull origin index
git pull origin contact
git push origin css
git checkout css
ip a

git add style.css
git commit -m "ici le push contient le fichier style.css pour l'index avec flex et les couleurs sunset"
git config user.email "antoine.haugazeau@efrei.net"
git config user.name "gearpimento"
git push -u origin css

git add stylec.css
git add stylec.css
git commit -m "fichier css de le fiche contact"
push -u origin css
```


