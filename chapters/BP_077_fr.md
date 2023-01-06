---
title :  Minifier les fichiers CSS, JavaScript, HTML et SVG
GreenIT : 12
Weight : 77
category : Production
tiers : Réseau
responsable : Architecte Logiciel/Développeur
priority: 4
difficulty: 3
impact: 4
ressources:
- Réseau
- Requêtes
gr491Recommandation : "BACK-END 3. Limiter la volumétrie des échanges"
gr491Critere : https://gr491.isit-europe.org/crit.php?id=3-7041-backend-les-echanges-indispensables-doivent-permettre-de-reduire
lighthouse : [unminified-css, unminified-javascript, unused-css-rules, unused-javascript]
tag : [ Incontournable, BACK-END ]
---

## Minifier les fichiers CSS, JavaScript, HTML et SVG

### Identifiants

| GreenIT |  V2  |  V3  |  V4  |
|:-------:|:----:|:----:|:----:|
|  12    | 78  | 77  |      |

### Catégories

| Cycle de vie |  Tiers  |  Responsable  |
|:---------:|:----:|:----:|
| 4. Production | Réseau | Architecte Logiciel/Développeur |

### Indications

| Degré de priorité |      Mise en oeuvre       |  Impact écologique    |
|:-------------------:|:-------------------------:|:---------------------:|
| 4 | 3 | 4 |

|Ressources Economisées                                      |
|:----------------------------------------------------------:|
| Réseau   |

### Description

Utiliser un outil de minification CSS, JavaScript, HTML et SVG permet de supprimer les espaces inutiles, les commentaires des développeurs, les sauts de ligne, les délimiteurs de blocs et ainsi réduire leur taille.

### Exemple

Il existe différents outils pour minifier comme par exemple:

- CSS: cssnano, csso ou clean-css 
- JavaScript: Terser, UglifyJS ou Babel-minify 
- HTML: htmlnano, HTMLMinifier
- SVG: SVGO, minify-xml ou équivalent


### Principe de validation

| Le nombre ...     | est inférieur ou égal à   |  
|-------------------|:-------------------------:|
| de fichiers CSS, JavaScript, HTML et SVG non minifiés  | 0  |
