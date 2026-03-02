# 🫀 Predictive Modeling for Heart Disease Diagnosis

Ce projet explore l'utilisation du Machine Learning pour diagnostiquer les maladies cardiaques en comparant une approche clinique manuelle à une optimisation algorithmique.

## 📌 Présentation du Projet
L'objectif est d'identifier les indicateurs clés des pathologies cardiovasculaires à partir de 270 cas cliniques et 13 caractéristiques prédictives. Nous cherchons à répondre à la question : *Le machine learning peut-il surpasser l'intuition clinique humaine ?*.

## 📊 Le Dataset
Le jeu de données comprend 270 observations sans valeurs manquantes ni doublons.
* **Variables Démographiques :** Âge, Sexe.
* **Symptômes :** Type de douleur thoracique, angine induite par l'effort.
* **Mesures Médicales :** Tension artérielle, Cholestérol, Glycémie (FBS), ECG, Fréquence cardiaque max (Max HR), dépression ST.
* **Variable Cible :** 'Heart Disease' (0 : Absence, 1 : Présence).

## 🛠 Méthodologie et Analyse
### 1. Analyse Statistique & Élagage
Nous avons effectué des tests de Student (données numériques) et du Chi-Carré (données catégorielles) pour filtrer les variables.
* **Variables Significatives :** Thallium, Max HR, Dépression ST, Nombre de vaisseaux, Type de douleur, etc.
* **Variables Exclues :** Le Cholestérol et la Glycémie (FBS) ont été retirés car ils n'étaient pas statistiquement significatifs pour ce modèle de prédiction précis.

### 2. Protocole Manuel (Intuition Clinique)
Un protocole basé sur des règles de décision humaine a été établi pour simuler un diagnostic médical :
* **Règle 1 :** Focus sur le Thallium et le nombre de vaisseaux.
* **Règle 2 :** Confirmation par la fréquence cardiaque et la dépression ST.
* **Précision obtenue :** 79.63%.

### 3. Optimisation par Machine Learning
Pour améliorer les résultats, nous avons utilisé un **Decision Tree Classifier** optimisé via **GridSearchCV** (testant 90 combinaisons de paramètres).

## 🚀 Résultats Finaux
| Méthode | Précision |
| :--- | :---: |
| Protocole Manuel (Humain) | 79.63% |
| **Modèle Final (IA)** | **94.44%** |

Le passage à un modèle optimisé permet d'atteindre une précision de **94.44%**, prouvant que l'IA est un outil complémentaire puissant pour détecter des signaux complexes dans les données cardiovasculaires.

## 👥 Auteurs
* **AL KHATIB Lara**
* **BOUAOUISS Rim**
