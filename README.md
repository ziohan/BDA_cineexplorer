# BDA_cineexplorer
CineExplorer est une application web hybride (Django/MongoDB/SQLite) permettant d'explorer une base de données de films enrichie et d'analyser les tendances du cinéma.

##  Fonctionnalités
- **Catalogue complet** : Filtrage par genre, année et note.
- **Moteur de recherche** : Recherche textuelle optimisée via MongoDB.
- **Statistiques interactives** : Visualisation de données avec Chart.js.
- **Architecture Hybride** : Utilisation conjointe de SQL (SQLite) et NoSQL (MongoDB).

##  Installation
1. Cloner le projet : `git clone https://github.com/ziohan/BDA_cineexplorer`
2. Créer un environnement virtuel : `python -m venv venv`
3. Installer les dépendances : `pip install -r requirements.txt`
4. Lancer le serveur : `python manage.py runserver`

##  Architecture NoSQL
Le projet utilise une stratégie de **dénormalisation** dans MongoDB (collection `MOVIES_FINAL`) pour optimiser les performances d'affichage des fiches détaillées (suppression des jointures).

###  Configuration MongoDB (Replica Set)
Le projet nécessite un Replica Set nommé `rs0` tournant sur les ports 27018, 27017 et 27019.
La connexion se fait via l'URI : `mongodb://localhost:27018,localhost:27019,localhost:27020/?replicaSet=rs0`

Le reste du code sera envoyé par mail à cause d'un problème sur github et sera à ajouter au repertoire principal.
