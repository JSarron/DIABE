# Projet DIABE : modélisation biomasse E. robusta dans les Hautes Terres Centrales de Madagascar


Ce projet fait référence à l'analyse de données de biomasses d'E. robusta dans le cadre du projet **DIABE**. 

**Collecteur des données** : Iviantsoa RAMANANDRAIBE
**Analyse et rédaction script** : Julien SARRON (Cirad - HortSys)
**Article associé** : 'Allometry and UAV-based estimation of tree dimensions, volume and aboveground biomass of Eucalyptus robusta plantations in the central highlands of Madagascar'


Le premier objectif de ce travail est de construire des relations allométriques pour les biomasses chaque compartiement et le volume (cubage) à partir des données de thèse de Iavantsoa Ramanandraibe (projet DIABE) et sans considérer les traitements âge et fertilisation (NF et F).
Le second objectif consiste à évaluer les potentialités du drone pour estimer la stucture des arbres (hauteur, volume, biomasse) et la biomasse totale des parcelles. Pour ce faire les parcelles ont été suvolées par un drone permettant la production de carte 3D. Puis les données drones sont comparées à des données de terrain (ground truth) pour calibrer des modèles. 

Il contient les script R et les données suivante :  

## Script pour l'établissement des relations allométriques 

**Nom du fichier** : *relation_allométrique.Rmd*

Script contenant les codes R pour établir les relations allométriques des arbres pour les biomasses feuilles, branche, tronc et total ainsi que le volume tous traitements confondus (age x fertilisation). 

Les relations sont d'abord calibrées sur l'ensemble des arbres prélevés (soit 64 arbres) puis sur les arbres qui ont été repéré par drone (40 arbres)

Ce script est associé à la base de données (.csv) *data_biomass_destructive* qui regroupe l'ensemble des données de biomasses et volume destructive par compartiment ainsi que l'analyse des échantillons de ces biomasses pour estimer les teneurs en eau

Le fichier permet de faire apparaître les sorties des modèles et les graphiques. 

## Script pour l'établissement des modèles drones 

**Nom du fichier** : *relation_allométrique.Rmd*

Script contenant les codes R pour établir les modèles drones pour estimer les biomasses et volumes touts traitement confondus

Ce script est associé à la base de données (.csv) *data_uav_calibration_tree* qui contient les données drones des 40 arbres échantillonés