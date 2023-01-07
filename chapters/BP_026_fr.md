---
title :  Utiliser les notations CSS abrégées
GreenIT : 15
Weight : 26
activity : Réalisation
tiers : Réseau
responsable : Architecte Logiciel/Développeur
priority: 2
difficulty: 3
impact: 2
ressources:
- Réseau
gr491Recommandation : "FRONT-END 9. Implémenter des solutions techniques dont l'impact est le plus faible"
gr491Search : https://gr491.isit-europe.org?famille=frontend&num_reco=9
mesurer : Le nombre de notations CSS non abrégés
tag : [ FRONT-END , FRONT-END, CSS ]
---

## Utiliser les notations CSS abrégées

### Identifiants

| GreenIT |  V2  |  V3  |  V4  |
|:-------:|:----:|:----:|:----:|
|   15   | 29  | 26  |      |

### Catégories

| Cycle de vie |  Tiers  |  Responsable  |
|:---------:|:----:|:----:|
| 3. Réalisation (fabrication / développement) | Réseau | Architecte Logiciel/Développeur |

### Indications

| Degré de priorité |      Mise en oeuvre       |  Impact écologique    |
|:-------------------:|:-------------------------:|:---------------------:|
| 2 | 3 | 2 |

|Ressources Economisées                                      |
|:----------------------------------------------------------:|
|  Réseau  |

### Description

Utiliser les notations CSS abrégées pour réduire le poids de la feuille de styles.

### Exemple

Ne pas écrire :
```css
margin-top:1em; margin-right:0; margin-bottom:2em; margin-left:0.5em;
```
mais plutôt :
```css
margin:1em 0 2em 0.5em;
```

Pour aller plus loin :
 - https://www.w3.org/TR/CSS
 - https://www.456bereastreet.com/archive/200502/efficient_css_with_shorthand_properties/

### Principe de validation

| Le nombre ...     | est inférieur ou égal à   |  
|-------------------|:-------------------------:|
| de notations CSS non abrégés  |  0% |
