# 🇲🇦 Morocco EduData Platform | منصة بيانات التربية والتعليم بالمغرب

> **L'Écosystème Numérique Unifié pour l'Extraction, la Modélisation et l'Analyse des Indicateurs Éducatifs et Évaluations Internationales au Maroc (1990–2024)**

[![Vercel Deployment](https://img.shields.io/badge/Deployed%20with-Vercel-black?style=for-the-badge&logo=vercel)](https://morocco-edudata-platform.vercel.app)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge)](LICENSE)
[![Status: Production](https://img.shields.io/badge/Status-Production%20Ready-success?style=for-the-badge)](#)

---

## 📌 Présentation Générale / Overview

**Morocco EduData Platform** est une infrastructure de données éducatives conçue pour les chercheurs, économistes, décideurs et data scientists. Elle unifie plus de **1 200 séries chronologiques** issues de 5 sources officielles (Banque Mondiale, UNESCO UIS, HCP, Ministère de l'Éducation Nationale MENPS et portail national data.gov.ma) avec une granularité territoriale couvrant les **12 régions et 75 provinces du Royaume**.

---

## ⚡ Fonctionnalités Clés / Key Features

1. **📊 Explorateur de Données Interactif (Data Explorer)**
   - Plus de 1 200 enregistrements pluriannuels (1990–2024).
   - Recherche prédictive plein texte et filtrage par thématique (Ressources Humaines, Organismes Internationaux, HCP, Scolarisation, Décrochage, Finances).
   - Pagination dynamique haute performance (15, 25, 50, 100 enregistrements).
   - Téléchargement granulaire indépendant à la ligne (*Row-by-Row Excel & CSV*).

2. **📈 Modélisation Temporelle & Courbes d'Évolution (Interactive Chart Modal)**
   - Un clic sur n'importe quel indicateur ouvre sa trajectoire historique complète.
   - Bascule fluide entre courbe continue (*Line*) et histogramme (*Bar*).
   - Calcul temps réel des 4 métriques de synthèse : **Dernière Valeur**, **Pic Historique (Max)**, **Plancher (Min)** et **Taux de Croissance Global**.
   - Tableau chronologique des variations annuelles (*YoY Delta*) et export dédié.

3. **🎯 Évaluations des Apprentissages (International & National Benchmarks)**
   - Données officielles **PISA** (OCDE, cycles 2018 et 2022) : Mathématiques, Sciences, Lecture et seuils de compétence.
   - Séries historiques **TIMSS & PIRLS** (IEA, 2011–2021) pour les 4e primaire et 2e collège.
   - Résultats du **Programme National PNEA** (Conseil Supérieur de l'Éducation CSEFRS).
   - Dictionnaire des variables (*Codebook*) avec définitions scientifiques et formules.

4. **🗺️ Observatoire Territorial des 12 Régions**
   - Disparités régionales et provinciales (Recensements RGPH du HCP).
   - Taux de scolarisation en milieu rural, analphabétisme et parité filles/garçons.

5. **☀️/🌙 Mode Jour / Nuit (Light / Dark Theme)**
   - Bascule instantanée entre thème sombre haute visibilité et thème clair éclatant.
   - Mémorisation automatique du choix utilisateur via `localStorage`.

6. **📗 Formats Dédiés à la Recherche Économétrique**
   - Données formatées et nettoyées (UTF-8 strict) pour importation immédiate sous **SPSS**, **R**, **Stata** et **Python**.

---

## 📁 Structure du Dépôt / Repository Structure

```
morocco-edudata-platform/
├── index.html                   # Application monopage complète et interactive
├── vercel.json                  # Configuration de déploiement et sécurité Vercel
├── README.md                    # Documentation complète
├── data/                        # Jeux de données bruts complets
│   ├── Morocco_EduData_Complete_1200_Records_Raw.csv
│   ├── Morocco_World_Bank_All_Education_Indicators_1990_2024.csv
│   └── DataGovMa_Education_Datasets_Catalog_API.csv
└── presentation/                # Présentations exécutives (PowerPoint)
    ├── Morocco_EduData_Platform_Presentation_FR.pptx
    └── Morocco_EduData_Platform_Presentation.pptx
```

---

## 🚀 Déploiement Local / Run Locally

Il suffit d'ouvrir le fichier `index.html` dans n'importe quel navigateur moderne, ou d'utiliser un serveur local :

```bash
# Avec Python
python -m http.server 3000

# Avec Node.js (npx serve)
npx serve .
```

---

## 🏛️ Sources Officielles des Données

- **Banque Mondiale (World Bank EdStats & HCI)** : [worldbank.org](https://data.worldbank.org)
- **UNESCO Institute for Statistics (UIS)** : [uis.unesco.org](https://uis.unesco.org)
- **Haut-Commissariat au Plan (HCP)** : [hcp.ma](https://www.hcp.ma)
- **Ministère de l'Éducation Nationale, du Préscolaire et des Sports (MENPS)** : [men.gov.ma](https://www.men.gov.ma)
- **Conseil Supérieur de l'Éducation, de la Formation et de la Recherche Scientifique (CSEFRS)** : [csefrs.ma](https://www.csefrs.ma)
- **Portail National des Données Ouvertes** : [data.gov.ma](https://data.gov.ma)

---

## 📜 Licence

Distribué sous licence **MIT**. Libre d'utilisation pour la recherche académique, l'enseignement et le développement de politiques publiques.
