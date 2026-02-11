# 📊 Analyse 360° E-Commerce : Stratégie & Risques (Olist Dataset)

## 📌 Présentation du Projet
Ce projet consiste en une analyse approfondie des données de la marketplace **Olist** (Brésil). L'objectif est de transformer des données brutes en insights actionnables pour quatre départements clés : **Marketing, Finance, Retail et Assurance.**

L'analyse couvre l'intégralité du cycle de vie d'une commande, de l'achat à la livraison, en intégrant la satisfaction client et la performance logistique.

---

## 🛠️ Stack Technique
- **SQL (BigQuery)** : Nettoyage, jointures complexes, segmentation RFM et création d'une table maîtresse (`master_reporting`).
- **Python (Pandas/Matplotlib)** : Analyse exploratoire (EDA) et détection des anomalies de données.
- **Tableau & Looker Studio** : Visualisation de données et dashboards interactifs.

---

## 🏛️ Les 4 Piliers de l'Analyse

### 1. Finance (Chiffre d'Affaires & Rentabilité)
- **Objectif** : Identifier la valeur générée par client.
- **Insight Clé** : Détection de "Power Users" (ex: un client ayant dépensé plus de 7 000 BRL), permettant de mesurer la concentration du CA sur les segments VIP.

### 2. Marketing (Fidélisation & RFM)
- **Objectif** : Segmenter la base client pour cibler les campagnes.
- **Insight Clé** : Création d'une segmentation **RFM** (Récence, Fréquence, Montant) corrigée en fonction de la chronologie réelle du dataset (Octobre 2018).

### 3. Retail (Performance Produit & Logistique)
- **Objectif** : Optimiser le catalogue et les flux.
- **Insight Clé** : Identification de catégories comme `cama_mesa_banho` (Linge de maison) qui génèrent un volume critique de plaintes malgré une livraison efficace.

### 4. Assurance & Risque (Qualité & Litiges)
- **Objectif** : Anticiper l'insatisfaction et les retours.
- **Insight Clé** : Analyse du **"Paradoxe de la Qualité"** : prouver par la donnée que certaines catégories de produits déçoivent à cause de leur qualité intrinsèque et non à cause des délais de livraison.

---

## 📈 Résultats Majeurs
- **Diagnostic Logistique** : Les retards de livraison impactent la note de satisfaction de manière exponentielle dès le 3ème jour de retard.
- **Opportunité Business** : Améliorer le contrôle qualité sur les catégories à fort volume et faible note pourrait réduire les coûts de service après-vente de manière significative.

---

## 📂 Structure du Repository
- `/sql` : Scripts de nettoyage, segmentation RFM et diagnostic de satisfaction.
- `/notebooks` : Analyse exploratoire et data cleaning via Python.
- `/dashboards` : Screenshots et liens vers les rapports interactifs (Tableau/Looker).

---

## 🚀 Comment utiliser ce projet
1. Importez les fichiers SQL dans BigQuery pour recréer la table `master_reporting`.
2. Connectez la table à Tableau ou Looker Studio en suivant les dimensions de satisfaction créées.
