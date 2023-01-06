---
title :  Utiliser certains forks applicatifs orientés "performance"
GreenIT : 4
Weight : 16
category : Réalisation
tiers : Datacenter
Responsable : Administrateur systèmes
priority: 3
difficulty: 3
impact: 3
ressources:
- Processeur
- Mémoire vive
- Réseau
gr491Recommandation : "BACK-END 2. Utiliser les composants techniques qui améliorent les aspects NR, sécurité et performance"
gr491Search : https://gr491.isit-europe.org?famille=backend&num_reco=2
tag : [ BACK-END ]
---

## Utiliser certains forks applicatifs orientés "performance"

### Identifiants

| GreenIT |  V2  |  V3  |  V4  |
|:-------:|:----:|:----:|:----:|
|  4    | 53  | 16  |      |

### Catégories

| Cycle de vie |  Tiers  |  Responsable  |
|:---------:|:----:|:----:|
| 3. Réalisation (fabrication / développement) | Datacenter | Administrateur systèmes |

### Indications

| Degré de priorité |      Mise en oeuvre       |  Impact écologique    |
|:-------------------:|:-------------------------:|:---------------------:|
| 3 | 3 | 3 |

|Ressources Economisées                                      |
|:----------------------------------------------------------:|
|  Processeur / Mémoire vive / Réseau  |

### Description

Les logiciels open source sont souvent « forkés » (dérivés) pour des raisons de performance. Or un gain de performance implique
généralement une réduction en termes de consommation de ressources. Par conséquent, si un fork optimisé existe et offre 
un périmètre fonctionnel et technique suffisant pour votre projet, vous devez l’utiliser.

### Exemple

 - À Drupal, préférer plutôt la version optimisée Pressflow.
 - À Redis, préférer plutôt la version optimisée KeyDB.

### Principe de validation

| Le nombre ...     | est inférieur ou égal à   |  
|-------------------|:-------------------------:|
| de forks orientés performance est supérieur ou égal à   | 1  |
