---
title :  Stocker les données dans le cloud
GreenIT : 71 
Weight : 93
category : Production
tiers : Datacenter
responsable : Administrateur systèmes
priority: 2
difficulty: 3
impact: 2
ressources:
- Stockage
gr491Recommandation : "STRATEGIE 8. Agir en faveur de la réduction des impacts du SI en optimisant la valorisation de la data (*NEW)"
gr491Critere : https://gr491.isit-europe.org/crit.php?id=8-1081-strategie-que-ce-soit-pour-le-si-operationnel
tag : [ STRATEGIE, Data ]
---

## Stocker les données dans le cloud

### Identifiants

| GreenIT |  V2  |  V3  |  V4  |
|:-------:|:----:|:----:|:----:|
|  71    |  92 |  93 |      |

### Catégories

| Cycle de vie |  Tiers  |  Responsable  |
|:---------:|:----:|:----:|
| 4. Production | Datacenter | Administrateur systèmes |

### Indications

| Degré de priorité |      Mise en oeuvre       |  Impact écologique    |
|:-------------------:|:-------------------------:|:---------------------:|
| 2 | 3 | 2 |

|Ressources Economisées                                      |
|:----------------------------------------------------------:|
| Stockage   |

### Description

Pour optimiser l’espace de stockage nécessaire aux ressources d’un site web ou d’un service en ligne, il peut être intéressant d’utiliser des solutions de cloud computing. Ainsi, tout en disposant d’une solution évolutive (elastic en anglais), on ne monopolise pas de ressources inutilement. L’autre intérêt est d’héberger les ressources statiques sur un domaine sans cookies. On évite alors de transporter le cookie avec chaque ressource transférée vers le navigateur (voir la bonne pratique n° 96).

Cette approche est donc judicieuse pour les images et autres ressources statiques. Comme il ne faut pas multiplier les domaines (voir la bonne pratique n° 55), le plus simple est de regrouper toutes les ressources statiques sur un seul service de stockage en ligne.

### Exemple

Pour la réalisation d’un jeu concours basé sur des témoignages vidéo, il est plus efficace de recourir au service de stockage S3 d’Amazon que d’ajouter de nouveaux disques durs aux serveurs existants.

### Principe de validation

| Le nombre ...     | est inférieur ou égal à   |  
|-------------------|:-------------------------:|
| de ressources, données du site web qui ne sont pas stockées sur une solution de cloud computing  |  0 |
