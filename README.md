# 🛠️ Projet Symfony – Gestion des Équipements

**Réalisé par : Cecilia Mendil**  
Projet développé avec le framework Symfony (PHP) et une base de données MySQL.

---

## 📘 Présentation générale

Ce projet est une application web développée avec **Symfony**, conçue pour gérer une liste d’équipements.  
Il simule une petite interface de gestion avec des pages dynamiques générées via le moteur de templates **Twig**.

Le projet est structuré selon le **modèle MVC** :  
- Les **Contrôleurs** assurent la logique métier et la gestion des routes  
- Les **Entités** et **Repositories** représentent la structure de la base de données et les opérations de récupération  
- Les **Vues Twig** assurent le rendu HTML des pages

Le projet utilise une **base de données MySQL**, dont la structure est incluse dans le fichier `cecilia.sql`, permettant une importation rapide dans phpMyAdmin ou tout autre outil SQL.

---

## 🎯 Objectifs pédagogiques

Ce projet m’a permis de mettre en pratique les compétences suivantes :

- Création d’une base de données relationnelle et structuration des tables
- Utilisation du framework Symfony (routes, contrôleurs, entités, vues)
- Utilisation de Doctrine pour la gestion des entités et des migrations
- Génération de templates HTML dynamiques avec Twig
- Application des bonnes pratiques de développement MVC

---

## 🧩 Fonctionnalités principales

- ✔️ Affichage dynamique de données à partir de la base MySQL
- ✔️ Organisation multi-pages à travers différents contrôleurs (`Page1Controller`, `Page2Controller`)
- ✔️ Intégration de templates personnalisés (`base.html.twig`, `index.html.twig`, etc.)
- ✔️ Utilisation de Doctrine pour gérer les migrations (table `doctrine_migration_versions`)
- ✔️ Importation facile de la structure de base via le fichier `cecilia.sql`

---

## 🗂️ Arborescence du projet

```bash
PROJET-SYMFONY/
│
├── config/                        # Fichiers de configuration Symfony
├── public/                        # Point d’entrée HTTP (web root)
├── src/                           # Dossier source du code PHP
│   ├── Controller/                # Logique métier (MVC)
│   │   ├── EquipmentController.php
│   │   ├── Page1Controller.php
│   │   └── Page2Controller.php
│   ├── Entity/                    # Définition des entités Doctrine
│   └── Repository/                # Requêtes personnalisées
│
├── templates/                     # Fichiers HTML Twig
│   └── equipement/
│       ├── index.html.twig
│       ├── page1.html.twig
│       ├── page2.html.twig
│       └── base.html.twig
│
├── cecilia.sql                    # Script SQL pour créer la base et les tables
├── .gitignore                     # Fichiers à exclure du suivi Git
├── composer.json                  # Dépendances PHP du projet
└── README.md                      # Documentation actuelle
