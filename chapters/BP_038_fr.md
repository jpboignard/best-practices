---
title :  Utiliser le rechargement partiel d'une zone de contenu
GreenIT : 40
Weight : 38
activity : Réalisation
tiers : Réseau
responsable : UX/UI Designer
priority: 4
difficulty: 3
impact: 4
ressources:
- Processeur
- Mémoire vive
- Réseau
tag : [ GR491-NOT-FOUND, FRONT-END ]
---

## Utiliser le rechargement partiel d'une zone de contenu

### Identifiants

| GreenIT |  V2  |  V3  |  V4  |
|:-------:|:----:|:----:|:----:|
|  40    |  49 | 38  |      |

### Catégories

| Cycle de vie |  Tiers  |  Responsable  |
|:---------:|:----:|:----:|
| 3. Réalisation (fabrication / développement) | Réseau | UX/UI Designer |

### Indications

| Degré de priorité |      Mise en oeuvre       |  Impact écologique    |
|:-------------------:|:-------------------------:|:---------------------:|
| 4 | 3 | 4 |

|Ressources Economisées                                      |
|:----------------------------------------------------------:|
| Processeur / Mémoire vive / Réseau   |

### Description

Si votre page web comporte une ou plusieurs zones de contenus qui nécessitent un taux de rafraîchissement élevé, alors nous vous conseillons de procéder à un rechargement uniquement de celles-ci et non pas de toute la page.
Pour cela vous pouvez utiliser plusieurs techniques généralement JavaScript couramment appelées AJAX mais qui peuvent aussi utilisées un Service Worker, un Web Component ou un développement sur mesure.

Il est même envisageable de ne pas inclure ces parties dans l'appel HTTP de la page pour l'hydrater avec ces zones dynamiques en JavaScript, ce que certains appellent "component islands" ou "islands architecture". L'intérêt étant de pouvoir conserver une solution de cache pour la page "container" et de ne recharger que les "ilots" de contenu qui le nécessitent.

### Exemple

Les sites d’actualité utilisent très souvent ce procédé, qui permet d’identifier clairement les zones qui nécessitent 
d’être mises à jour rapidement (flash d’informations, données météo, cours de la Bourse, résultats sportifs, etc.).

### Principe de validation

| Le nombre ...     | est inférieur ou égal à   |  
|-------------------|:-------------------------:|
| de zones de contenu pouvant être mis à jour partiellement mais qui ne le sont pas  | 0%  |
