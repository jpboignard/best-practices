---
title : Créer une architecture applicative modulaire
GreenIT : 114
Weight : 14
activity : Conception
tiers : Datacenter
responsable : Architecte Logiciel/Développeur
priority: 3
difficulty: 3
impact: 3
ressources:
- Processeur
- Mémoire vive
- Stockage
gr491Recommandation : "ARCHITECTURE 6. Définir un modèle de production évolutif"
gr491Critere : https://gr491.isit-europe.org/crit.php?id=6-6031-architecture-les-efforts-dadaptation-aux-contraintes-environnementales-realises
tag : [ Recommandation, ARCHITECTURE ]
---

## Créer une architecture applicative modulaire

### Identifiants

| GreenIT |  V2  |  V3  |  V4  |
|:-------:|:----:|:----:|:----:|
|  114    | 52  | 14  |      |

### Catégories

| Cycle de vie |  Tiers  |  Responsable  |
|:---------:|:----:|:----:|
| 2. Conception | Datacenter | Architecte Logiciel/Développeur |

### Indications

| Degré de priorité |      Mise en oeuvre       |  Impact écologique    |
|:-------------------:|:-------------------------:|:---------------------:|
| 3 | 3 | 3 |

|Ressources Economisées                                      |
|:----------------------------------------------------------:|
|  Processeur / Mémoire vive / Stockage  |

### Description

L’architecture modulaire popularisée par les logiciels open source apporte souvent une plus grande capacité à monter en charge,
des coûts réduits de maintenance corrective et évolutive, ainsi qu’un code plus efficient.
Si la couverture fonctionnelle du site web ou du service en ligne peut être amenée à évoluer, mieux vaut implémenter les fonctionnalités de base dans un noyau et les compléter au besoin par des modules. Ces modules peuvent rassembler des fonctions appartenant à un même domaine métier. Cela permet de les développer indépendamment des autres domaines métier ainsi que les partager à d'autres applications.

Cette approche est valable à tous les niveaux de granularité, pour un développement sur mesure comme pour le choix d’un serveur HTTP ou d’un CMS.

### Exemple

Les logiciels open source les plus efficients, comme nginX, Apache, MySQL ou PHP, reposent sur cette architecture modulaire.

Côté backend, le découpage en microservices permet d'apporter un niveau de modularité pour des services HTTP. Il faudra néanmoins porter une attention particulière sur la granularité du découpage pour éviter un effet contre-productif (ajout d'une complexité d'interfaçage entre les services, augmentation globale des ressources informatiques).

### Principe de validation

| Le nombre ...     | est inférieur ou égal à   |  
|-------------------|:-------------------------:|
| Le nombre d'architectures non modulaires | 0  |
