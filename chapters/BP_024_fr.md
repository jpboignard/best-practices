---
title :  Ecrire des sélecteurs CSS efficaces
GreenIT : 13
Weight : 24
activity : Réalisation
tiers : Réseau
responsable : Architecte Logiciel/Développeur
priority: 3
difficulty: 3
impact: 2
ressources:
- Processeur
gr491Recommandation : "FRONT-END 9. Implémenter des solutions techniques dont l'impact est le plus faible"
gr491Search : https://gr491.isit-europe.org?famille=frontend&num_reco=9
mesurer : Le nombre de sélecteurs CSS qui n'utilisent ni d'id, ni de class et ni d'attribut
tag : [ FRONT-END, CSS ]
---

## Écrire des sélecteurs CSS efficaces

### Identifiants

| GreenIT |  V2  |  V3  |  V4  |
|:-------:|:----:|:----:|:----:|
|  13    | 27  | 24  |      |

### Catégories

| Cycle de vie |  Tiers  |  Responsable  |
|:---------:|:----:|:----:|
| 3. Réalisation (fabrication / développement) | Réseau | Architecte Logiciel/Développeur |

### Indications

| Degré de priorité |      Mise en oeuvre       |  Impact écologique    |
|:-------------------:|:-------------------------:|:---------------------:|
| 3 | 3 | 2 |

|Ressources Economisées                                      |
|:----------------------------------------------------------:|
|  Processeur  |

### Description

Privilégier les sélecteurs basés sur des ID ou des classes. Ils seront ainsi filtrés plus rapidement, économisant des cycles CPU à la machine interprétant les règles.

### Exemple

Ne pas écrire :
```css
treeitem[mailfolder="true"] > treerow > treecell {…}
```
mais plutôt :
```css
.treecell-mailfolder {…}
```

Ne pas écrire :
```css
treehead > treerow > treecell {…}
```
mais plutôt :
```css
.treecell-header {…}
```

### Principe de validation

| Le nombre ...     | est inférieur ou égal à   |  
|-------------------|:-------------------------:|
| de sélecteurs CSS qui n'utilisent ni d'id, ni de class et ni d'attribut  |  0 |
