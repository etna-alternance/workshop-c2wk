# Workshop 🎵 : Construire une base de données relationnelle pour un service de musique similaire à Spotify

## 🏆 **Objectif**
Concevoir un modèle de base de données relationnelle efficace pour un service de streaming musical. Cet atelier vous guidera dans la définition des fonctionnalités, l'identification des entités et de leurs attributs, et la modélisation des interactions entre elles.

## **Étape 0 : Sites web utiles:**
Quelques outils qui peuvent être utiles pour concevoir votre base de données :

- Lucidchart : Un outil populaire de création de diagrammes.
- dbdiagram.io : Outil gratuit et open-source pour la création de diagrammes ER.

## **Étape 1 : Identifier les fonctionnalités clés**

Voici les principales fonctionnalités que notre service de type Spotify prendra en charge :
1. 🎧 **Lecture de musique** : Les utilisateurs peuvent lire des chansons en continu.
2. 👤 **Comptes d'utilisateur** : Les utilisateurs peuvent créer et gérer leurs profils.
3. 🔒 **Authentication** : Connexion sécurisée des utilisateurs.
4. 📜 **Listes de lecture** : Les utilisateurs peuvent créer et gérer des listes de lecture.
5. ❤️ **Système de favoris** : Les utilisateurs peuvent enregistrer leurs chansons préférées.
6. 💿 **Albums et artistes** : Les chansons sont regroupées dans des albums et liées à des artistes.
7. 🕒 **Historique d'écoute** : Suivre les chansons récemment écoutées.

## **Étape 2 : Définir les objets et les attributs**

### 🎶 **1. Chanson**
Représente une piste individuelle.

### 📋 **2. Liste de lecture**
Une collection de chansons créée par l'utilisateur.

### 👤 **3. Utilisateur**
Représente les titulaires de comptes du service.

### 💿 **4. Album**
Représente une collection de chansons d'un artiste.

### 🎤 **5. Artiste**
Représente un artiste individuel ou un groupe.

## **Étape 3 : Modéliser les relations**

### 💬 **Interactions des utilisateurs avec les chansons**
- Les utilisateurs peuvent aimer des chansons (relation plusieurs à plusieurs).
- Les utilisateurs peuvent écouter des chansons (lecture de pistes dans l'historique d'écoute).

### 🔗 **Chansons dans les listes de lecture**
- Une liste de lecture contient plusieurs chansons, et les chansons peuvent appartenir à plusieurs listes de lecture (relation plusieurs à plusieurs).

### 🎶 **Chansons, albums et artistes**
- Chaque chanson appartient à un album (relation de type « un à plusieurs »).
- Chaque chanson est interprétée par un artiste (relation de type « un à plusieurs »).
- Les albums sont créés par des artistes (relation de type « un à plusieurs »).
