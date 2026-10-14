# Analyse du marché Airbnb à Paris — rentabilité d'un investissement courte durée

Projet de Master 1 (Informatique & Big Data, Université Paris 8) réalisé avec **Tableau Public**.

## Problématique

L'investissement locatif de courte durée à Paris est-il rentable ? Quels quartiers privilégier, et quels leviers permettent de maximiser les revenus ?

## Données

- Annonces Airbnb issues de Kaggle ([airbnb-paris](https://www.kaggle.com/datasets/abaghyangor/airbnb-paris)), restreintes à **Paris (~65 000 annonces)**.
- Fichier complémentaire construit pour l'étude : **prix au m² approximatif par quartier** (absent du jeu de données d'origine).

## Méthode

- **Rendement brut annualisé** = (prix médian × 365 × taux d'occupation) / prix d'achat médian du quartier.
- Hypothèses : taux d'occupation de 65 %, logement de 40 m².
- **Médiane plutôt que moyenne** pour limiter l'effet des annonces premium.
- Analyse par **quartier administratif** (plus fin que l'arrondissement).

## Visualisations (9)

Treemap des types de logements, annonces par quartier, hôtes occasionnels vs professionnels, carte prix m² × prix/nuit × volume, comparaison Superhost vs hôte classique, nombre de Superhosts, scatter plot rendement × volume, prix par personne selon la capacité, évolution du nombre de nouveaux hôtes (2008-2021).

## Résultats

- Le quartier de **l'Élysée** ressort comme le plus opportun : rendement brut de **5,82 %** (Superhost) contre **5,43 %** (hôte standard), avec une faible pression concurrentielle.
- Le statut **Superhost** est un levier de performance majeur.
- Le marché est dominé par des hôtes occasionnels (plus de 46 000 annonces).

## Limites

Prix moyens par quartier qui lissent les écarts locaux, réglementation non prise en compte (limite de 120 jours par an pour une résidence principale), charges et fiscalité exclues (rendement net surestimé), taux d'occupation fixé arbitrairement, pas de distinction par surface.

## Contenu du dépôt

- `Airbnb_analyse.twbx` — classeur Tableau (à ouvrir avec Tableau Public / Desktop).
- `docs/Note_methodologique.pdf` — note méthodologique complète.

## Auteur

Yannick Jin — Master 2 Informatique & Big Data, Université Paris 8.
