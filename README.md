# git mémo


`/!\` Les informations contenues entre les symboles `<` et `>`

`/!\` sont à adapter celons votre utilisation sur les lignes commençant par des `$` bien sûr ^^

## ![Logo Doom godmod 38px](https://raw.githubusercontent.com/jplemonias/thp/master/img/godmode38.png)  Git version

Permet de connaite la version instalée de Git.

    $ git --version

juste :

    $ git

renvoi l'help de Git ( si instalé ).

-----------------

## ![Logo Doom suspect 38px](https://raw.githubusercontent.com/jplemonias/thp/master/img/suspect38.png) Git config


Permet de spécifier / connaitre les paramètres de configuration de Git avec la commande `git config`. 

    $ git config --global user.name < LoginGithub >
    $ git config --global user.email < MonEmail@mail.com >

Pour conaitre le nom utilisé et le mail :

    $ git config --global user.name 
    LoginGithub
    $ git config --global user.email
    MonEmail@mail.com

-----------------

## ![Logo Doom rage1 38px](https://raw.githubusercontent.com/jplemonias/thp/master/img/rage138.png) Git init

On crée un dossier git on si déplace et on initie le repo Gità l'aide de `git init`.

    $ mkdir git
    $ cd git

    $ git init
    
-----------------

## ![Logo Doom rage2 38px](https://raw.githubusercontent.com/jplemonias/thp/master/img/rage238.png) Git status

    $ git status

A ce stade indique :

    Sur la branche master
    Aucun commit
    rien à valider (créez/copiez des fichiers et utilisez "git add" pour les suivre)

-----------------

## ![Logo Doom rage3 38px](https://raw.githubusercontent.com/jplemonias/thp/master/img/rage238.png)  Git add

On crée un fichier `README.md`.

    $ touch README.md
    $ git add README.md
    $ git status

Le nouveau statut est :

    Sur la branche master
    Aucun commit
    Modifications qui seront validées :
        (utilisez "git rm --cached <fichier>..." pour désindexer)
	        nouveau fichier : README.md

-----------------

## ![Logo Doom rage4 38px](https://raw.githubusercontent.com/jplemonias/thp/master/img/rage438.png) Git commit

    $ git commit -m < "Creat README.md" >

Devrait renvoyer quelque chose comme cela :

    [master (commit racine) xx123yy] Création du fichier README.md
     1 file changed, 0 insertions(+), 0 deletions(-)
     create mode 100644 README.md

-----------------

## ![Logo Doom goberserk 38px](https://raw.githubusercontent.com/jplemonias/thp/master/img/goberserk38.png) Git branch

    $ git branch -M main

-----------------

## ![Logo Doom goberserk 38px](https://raw.githubusercontent.com/jplemonias/thp/master/img/goberserk38.png) Git remote

Par SSH :

    $ git remote add origin git@github.com:< LoginGithub >/git.git

Par HTTPS :

    $ git remote add origin https://github.com/< LoginGithub >/git.git

-----------------

## ![Logo Doom finnadie 38px](https://raw.githubusercontent.com/jplemonias/thp/master/img/finnadie38.png) Git push
    $ git push -u origin main

On écrit dans README.md puis on l'upload

    $ git commit -m < "Complet README.md part 1" >

Devrait renvoyer :

    [main 123a321] Complet README.md part 1
     1 file changed, 111 insertions(+), 0 deletions(-)
     rewrite README.md (100%)


Pe@cE