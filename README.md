# 📒 Notebooks de traitement — Architecture Médaillon

Ce dépôt contient les notebooks utilisés pour la mise en place d’une architecture de type *médaillon* (Bronze → Argent → Or). Chaque notebook correspond à une étape spécifique du pipeline de traitement des données.

---

## 🔹 Chargement fichier — Niveau Bronze

**Objectif :**  
Charger les fichiers sources depuis un stockage local.

**Détails :**  
- Intégration des données brutes sans transformation.
- Création de la table Delta.

---

## 🔸 Fusion fichiers — Niveau Argent

**Objectif :**  
Nettoyer et transformer les données intégrées.

**Détails :**  
- Fusion des fichiers sources.
- Ajout de colonnes enrichies.
- Nettoyage des données.
- Création de la table argent.

---

## 🟡 Dimension_tables — Niveau Or (Dimensions)

**Objectif :**  
Construire les tables de dimensions nécessaires aux analyses métier.

**Détails :**  
- Création des dimensions.
- Préparation des jointures futures avec la table de faits.

---

## 🟡 Fast_table — Niveau Or (Faits)

**Objectif :**  
Générer la table de faits à partir des données préparées.

**Détails :**  
- Agrégation des indicateurs clés.
- Constitution de la table centrale pour l’analyse (modèle en étoile).

---

## 🧱 À propos de l’architecture Médaillon

L’approche *médaillon* permet de structurer les pipelines de données en plusieurs couches :
- **Bronze** : Données brutes.
- **Argent** : Données nettoyées et enrichies.
- **Or** : Données modélisées et prêtes à l’analyse.

---
