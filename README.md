#  Mon Projet ML — Pipeline de Traduction Automatique

Projet réalisé dans le cadre du cours **Big Data et Infrastructure Machine Learning**.  
Ce projet consiste à intégrer et adapter un code existant dans un template Cookiecutter afin de construire un pipeline modulaire de traduction automatique.

---

##  Objectif du projet

L’objectif principal est de mettre en place un pipeline complet permettant de :

- Traduire des textes du français vers l’anglais à l’aide du modèle **Helsinki-NLP/opus-mt-fr-en** (HuggingFace)
- Évaluer la qualité des traductions avec la métrique **BLEU**
- Structurer le projet selon les bonnes pratiques d’ingénierie logicielle (modularité, lisibilité, testabilité)

---

##  Travail réalisé

Dans cette étape, le projet a été construit à partir du dépôt source suivant :

 https://github.com/delnouty/bidabi-clone-adapt-translate.git

Le template initial ne contenait qu’une structure vide. Le travail a consisté à :

- Cloner et analyser le dépôt fourni
- Comprendre l’organisation du code existant
- Intégrer les différentes briques dans les modules du template :
  - `loaders`
  - `processors`
  - `translators`
  - `evaluators`
  - `orchestrator`
- Adapter le code pour respecter l’architecture imposée par le template
- Vérifier le bon fonctionnement global du pipeline après intégration

Ce travail a été réalisé de manière autonome, en appliquant une démarche d’ingénierie logicielle rigoureuse.

---

##  Architecture du projet
Le projet est organisé de manière modulaire afin de séparer les responsabilités et faciliter la maintenance, l’évolution et la lisibilité du code.


---

##  Fonctionnement du pipeline

Le pipeline est orchestré par une classe centrale (`Orchestrator`) qui exécute les étapes suivantes :

1. Chargement des données depuis `data/`
2. Traduction des textes (fr → en)
3. Prétraitement éventuel des données
4. Évaluation des traductions via le score BLEU
5. Sauvegarde des résultats dans `output/`

---

##  Installation


git clone https://github.com/Jineneh/cookiecutter-ml-template.git
cd cookiecutter-ml-template
Compétences mobilisées
Structuration d’un projet Python modulaire
Intégration et adaptation de code existant
Utilisation de modèles HuggingFace
Traitement de données textuelles
Évaluation automatique (BLEU)
Bonnes pratiques Git et CI/CD
## Critères d’évaluation

Le projet est évalué selon :

-La qualité de l’intégration du code
-Le bon fonctionnement du pipeline
-La clarté et l’organisation du dépôt
-La qualité du README
-Le respect des conventions (tests, formatage, structure)
-La propreté du projet (Git, fichiers inutiles, etc.)
## Auteur

Jineneh

## Version Python

Python 3.10+
