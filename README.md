# HASKELL - 07/08/2021

## Installer sqlite3

### Récupérer le package

- Aller sur https://www.sqlite.org/download.html

- Dans "Precompiled Binaries for Windows"
  - download la package "sqlite-tools-win32-x86-3360000.zip (1.82 MiB)"

### Rendre Sqlite3 accessible en commande

- Dézipper le dossier downloadé précédemment dans "C:\sqlite3\"

- Indiquer le Path dans les variables système de Windows
  - Cliquer droit sur "Démarrer"
  - Ouvrir "Système"
  - Aller sur "Paramètre avancés du système"
  - Aller  sur "Variables d'environnement..."
  - Dans "Variables système", sélectionner "Path" puis cliquer sur "Modifier..."
  - Cliquer sur "Nouveau" pour ajouter le chemin "C:\sqlite3\"
  - Cliquer OK plusieurs fois pour valider

### Créer le fichier .DB
- Créer le dossier "\db" sur le bureau
- Cliquer droit sur "Démarrer"
- Ouvrir "invite de commmandes (admin)"
- Dans le shell de Windows :
  - Aller sous le dossier "\db"
    - $>cd C:\Users\WingQiqi\Desktop\db
  - Puis créer de fichier de base de données "mydb.db"
    - $>sqlite3 mydb.db"

### Quelques commandes sous $sqlite3
- Pour lister les commandes :
  - $sqlite>.help 

- Pour lister les base de données :
  - $sqlite>.database

- Pour créer la table "students" avec "id" comme clé primaire :
  - "$sqlite>create table students (id INT primary key)"

- Pour lister les tables :
  - $sqlite>.tables

- Pour lister la structure de la table "students" :
  - $sqlite>.schema students




