# Retail Sales & Business Performance Analytics

## Contexte

Ce projet simule une mission de Data Analytics réalisée pour une entreprise du secteur retail disposant de plusieurs années de données transactionnelles. L'entreprise commercialise différentes catégories de produits dans plusieurs régions. La direction souhaite comprendre les facteurs qui influencent son chiffre d'affaires et sa rentabilité afin d'identifier les produits, clients et zones géographiques les plus performants ou problématiques et de soutenir la prise de décision.

## Objectifs du projet

L'objectif du projet est d'analyser les performances commerciales de l'entreprise afin d'identifier les principaux leviers de croissance et de rentabilité et de formuler des recommandations basées sur les données. Plus en détails, nous allons :

- Analyser l'évolution des performances commerciales.
- Identifier les produits, catégories et zones géographiques les plus performants.
- Étudier la rentabilité des différentes activités.
- Analyser le comportement et la contribution des clients.
- Étudier l'impact des remises sur les performances.
- Construire un tableau de bord décisionnel permettant le suivi des principaux KPI.

## Questions métier

1. Comment évoluent le chiffre d'affaires et le profit dans le temps ?
2. Quelles catégories et sous-catégories génèrent le plus de chiffre d'affaires ?
3. Quelles catégories sont les plus ou les moins rentables ?
4. Quelles régions ou zones géographiques performent le mieux ?
5. Quels clients contribuent le plus aux performances commerciales ?
6. Existe-t-il des produits avec un chiffre d’affaires élevé mais une rentabilité faible ou négative ?
7. Quel est l'impact des remises sur la rentabilité ?
8. Existe-t-il des tendances saisonnières dans les ventes ?

## Dataset

Ce projet s'appuie sur le dataset **[Global Electronics Retailer](https://mavenanalytics.io/data-playground/global-electronics-retailer)**, qui simule l'activité commerciale d'une entreprise internationale spécialisée dans la vente de produits électroniques.

Le dataset permet de suivre les commandes réalisées par les clients dans différents magasins et pays. Pour chaque vente, il est notamment possible d'identifier le client, le produit acheté, la quantité commandée, le magasin ayant traité la commande, les dates de commande et de livraison ainsi que la devise utilisée. Des informations complémentaires sont également disponibles sur les caractéristiques des produits, leur prix de vente et leur coût, le profil géographique des clients, les magasins et les taux de change.

Les données sont réparties dans cinq tables métier principales :

- `Sales` : lignes de commandes et quantités vendues ;
- `Customers` : informations démographiques et géographiques sur les clients ;
- `Products` : catalogue des produits, marques, catégories, prix de vente et coûts ;
- `Stores` : localisation, surface et date d'ouverture des magasins ;
- `Exchange_Rates` : taux de change par date et devise.

Un sixième fichier, `Data_Dictionary`, documente les différents champs du dataset.

La table `Sales` constitue la table centrale du modèle. Son niveau de granularité correspond à la **ligne de commande** : une ligne représente un produit acheté au sein d'une commande. Elle est reliée aux autres tables par les identifiants du client, du produit et du magasin, ainsi que par la date et la devise pour les taux de change.

Ce dataset a été retenu car sa structure multi-tables permet de reproduire un cas d'analyse décisionnelle proche d'un environnement professionnel. Il offre notamment la possibilité d'étudier l'évolution des ventes, la rentabilité des produits, les performances géographiques et magasins ainsi que le comportement des clients, tout en mettant en pratique SQL, la modélisation dimensionnelle, la construction de KPI et la création d'un tableau de bord Power BI.

## Stack technique

La stack technique sera définie progressivement au cours du projet.

## Statut du projet

Projet en cours de construction.