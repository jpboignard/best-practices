---
title :  Découper les CSS
GreenIT : 9
Weight : 21
activity : Réalisation
tiers : Réseau
responsable : UX/UI Designer
priority: 4
difficulty: 4
impact: 4
ressources:
- Processeur
- Réseau
gr491Recommandation : "FRONT-END 9. Implémenter des solutions techniques dont l'impact est le plus faible"
gr491Search : https://gr491.isit-europe.org?famille=frontend&num_reco=9
mesurer : Le nombre de librairies CSS
tag : [ FRONT-END, CSS  ]
---

## Découper les CSS

### Identifiants

| GreenIT |  V2  |  V3  |  V4  |
|:-------:|:----:|:----:|:----:|
|   9   | 24  | 21  |      |

### Catégories

| Cycle de vie |  Tiers  |  Responsable  |
|:---------:|:----:|:----:|
| 3. Réalisation (fabrication / développement) | Réseau | UX/UI Designer |

### Indications

| Degré de priorité |      Mise en oeuvre       |  Impact écologique    |
|:-------------------:|:-------------------------:|:---------------------:|
| 4 | 4 | 4 |

|Ressources Economisées                                      |
|:----------------------------------------------------------:|
|  Processeur / Réseau  |

### Description

Employer un ensemble de CSS plutôt qu’une seule, et appeler uniquement les CSS utiles en fonction du contexte. 
Cette méthode permet de limiter le poids de la page lors du premier téléchargement, donc d’économiser de la bande passante 
et de réduire la charge CPU.

### Exemple

Découper les CSS en fonction de la logique fonctionnelle :
 - layout ;
 - content ;
 - module x ;
 - module y ;
 - etc...

Dans le cas d’un site fonctionnellement riche, cela permettra d’exclure toutes les CSS des modules non utilisés. 
Le nombre de CSS doit rester raisonnable, plus pour des questions de maintenabilité que de performance, 
dans la mesure où les CSS générales (« layout » et « content » dans notre exemple) seront concaténées en un seul fichier. 
Les CSS complémentaires (ici, « module x » et « module y ») seront téléchargées en fonction du contexte (page, fonctionnalités...).


### Principe de validation

| Le nombre ...     | est inférieur ou égal à   |  
|-------------------|:-------------------------:|
| de librairies CSS est supérieur ou égal  | 2  |
