# 📊 Projet Analyse de Données – README

## 👥 Auteurs

Antoine Malleret, Adrien Morille\
Date : 6 avril 2025

------------------------------------------------------------------------

## 🔍 Description générale

Ce projet d’analyse de données en R a pour but d’explorer, nettoyer et analyser un jeu de données, notamment :

-   Analyse en Composantes Principales (ACP)

-   Analyse Factorielle des Correspondances (AFC)

-   Classification non supervisée (k-means, hiérarchique, etc.)

-   Classification supervisée (Random Forest, LDA, QDA, etc.)

## 📁 Structure du projet

Le projet est structuré autour d’un **fichier principal `main.Rmd`**, qui sert de point d’entrée pour compiler l’ensemble du projet, et de plusieurs **fichiers `.Rmd` enfants** correspondant aux différentes étapes de l’analyse.

### 📜 Fichiers RMarkdown inclus

-   `main.Rmd` : script principal de compilation
-   `Introduction.Rmd` : présentation du projet et des données
-   `DataCleanning.Rmd` : nettoyage, sélection et préparation des données
-   `ACP.Rmd` : analyse en composantes principales
-   `AFC.Rmd` : analyse factorielle des correspondances
-   `Classification_non_supervisée.Rmd` : classification non supervisée
-   `ClassificationSupervisee.Rmd` : classification supervisée
-   `Conclusion.Rmd` : conclusion et perspectives
-   `Annex.Rmd` : expliquation des variables/colonnes du jeu de données
-   `Exploration.Rmd` : Exploration basique des données

------------------------------------------------------------------------

## ⚙️ Instructions de compilation

### 🔹 Étapes à suivre :

1.  **Charger les bibliothèques** (au début de `main.Rmd`)\
    Cela permet d’assurer que toutes les fonctions nécessaires sont disponibles.

2.  **Compiler `DataCleanning.Rmd` juste après**\
    Ce fichier est **indispensable**, car il charge et prépare les jeux de données qui seront utilisés dans toutes les autres parties.\
    **💡 Important : Cela permet de rendre les données disponibles en tant que variables locales dans l’environnement RMarkdown.**

3.  **Compiler ensuite librement les autres sections** selon les analyses souhaitées (ACP, classification, etc.).

------------------------------------------------------------------------

## 🧩 Modularity — Parties indépendantes

Toutes les parties du projet (`ACP`, `Classification`, etc.) sont **indépendantes entre elles**.\
Vous pouvez donc : - Exécuter uniquement une ou deux parties sans devoir compiler tout le projet.

------------------------------------------------------------------------

## ❗ Remarques

-   Le fichier `DataCleanning.Rmd` est la **seule dépendance obligatoire** : il doit être exécuté **avant toute autre analyse** pour garantir que les données sont bien présentes dans l’environnement.

------------------------------------------------------------------------

## 📚 Jeu de données

Le jeu de données utilisé dans ce projet à été extrait automatiquement depuis l'API de yahoo finance.\
Il s'agit d'un fichier CSV contenant des données financières sur les actions de plusieurs entreprises.\
Le fichier est divisé en plusieurs colonnes, chacune représentant une variable différente.\
Les données peuvent être fausse ou incomplètes.\

